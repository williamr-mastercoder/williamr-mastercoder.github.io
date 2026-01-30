const audio = document.getElementById("audio");
const playBtn = document.getElementById("playBtn");

// put your audio or stream link here
audio.src = "https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3";

let playing = false;

playBtn.onclick = () => {
  if (!playing) {
    audio.play();
    playBtn.innerText = "Pause";
    playing = true;
  } else {
    audio.pause();
    playBtn.innerText = "Play";
    playing = false;
  }
};
