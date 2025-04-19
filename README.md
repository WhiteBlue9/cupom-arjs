<!DOCTYPE html>
<html>
  <head>
    <title>Teste WebAR Geolocalizado</title>
    <script src="https://aframe.io/releases/1.2.0/aframe.min.js"></script>
    <script src="https://raw.githack.com/jeromeetienne/AR.js/3.3.2/aframe/build/aframe-ar.min.js"></script>
  </head>
  <body style="margin: 0; overflow: hidden;">
    <a-scene
      embedded
      arjs="sourceType: webcam; gpsMinDistance: 5;"
      vr-mode-ui="enabled: false"
      renderer="logarithmicDepthBuffer: true;"
    >

      <a-box 
        gps-entity-place="latitude: -23.550520; longitude: -46.633308;"
        color="red"
        scale="5 5 5"
      ></a-box>

      <a-camera gps-camera rotation-reader></a-camera>

    </a-scene>
  </body>
</html>
