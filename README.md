function getRandomColor() {
  const color = "#" + Math.floor(Math.random()*16777215).toString(16);
  return color.padEnd(7, '0'); // Ensures color code is always 7 characters
}

function changeColor() {
  const newColor = getRandomColor();
  const box = document.getElementById("colorBox");
  box.style.backgroundColor = newColor;
  box.textContent = newColor;
}
