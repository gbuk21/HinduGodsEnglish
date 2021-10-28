---
last_modified_at: 2021-10-28
layout: post
title: Lakshmi Kubera Mantras chant - whole day long
---
  <body>

    <!-- 1. The <iframe> (and video player) will replace this <div> tag. -->
    <div id="player"></div>

    <script>
      // 2. This code loads the IFrame Player API code asynchronously.
      var tag = document.createElement('script');
      var repeat_count = 0;
      var data = ['0xu7gwNZJd8', 'iCWrpDShdG4', 'yhMH-FbSfQM', 'FRklYmmmwYE', 'GD-O8bMkclk', 'nnXR0heG8SY', 'Oi8Y42WrP_Y']
      var data_index =0;
      tag.src = "https://www.youtube.com/iframe_api";
      var firstScriptTag = document.getElementsByTagName('script')[0];
      firstScriptTag.parentNode.insertBefore(tag, firstScriptTag);

      // 3. This function creates an <iframe> (and YouTube player)
      //    after the API code downloads.
      var player;
      function onYouTubeIframeAPIReady() {
        player = new YT.Player('player', {
          height: '600',
          width: '800',
          videoId: 'Oi8Y42WrP_Y',
          playerVars: {
            'autoplay': 1 
          },
          events: {
            'onReady': onPlayerReady,
            'onStateChange': onPlayerStateChange
          }
        });
      }

      // 4. The API will call this function when the video player is ready.
      function onPlayerReady(event) {
        event.target.playVideo();
      }

      // 5. The API calls this function when the player's state changes.
      //    The function indicates that when playing a video (state=1),
      //    the player should play for six seconds and then stop.
      var done = false;
      function onPlayerStateChange(event) {
        if (event.data == YT.PlayerState.PLAYING && !done) {
          done = true;

        }
        if (player.getPlayerState()==0) {
          player.loadVideoById(data[data_index])
          if (data_index <7) {
             data_index=data_index+1;
          } else {data_index=0;}
          player.play()
        }
      }
    </script>
  </body>
