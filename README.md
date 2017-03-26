Function() {
  var video = document.getElementById ('video'),
  vendorUrl = window.URL || window.webkitURL;
  navigator.getMedia = navigator.getUserMedia ||
                       navigator.WebkitGetUserMedia ||
					   navigator.mozGetUserMedia;
					   
navigator.getMedia ({
          video: true,
		  audio:true },
function(stream) {
video.src =vendorUrl.creatObjectURL(stream);
video.play();
},
function(Error){
//fyofuoguogoyf
});
};
