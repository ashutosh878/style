@import url('https://fonts.googleapis.com/css?family=Poppins');

* {
  font-family: 'Poppins', sans-serif;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  height: 100vh;
  overflow: hidden;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #d6b398;
}

.selectnone {
  -webkit-touch-callout: none;
  -webkit-user-select: none;
  -khtml-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
  -webkit-tap-highlight-color: transparent;
}

button {
  width: 150px;
  height: 50px;
  background: none;
  border: 2px solid #932e3e;
  border-radius: 50px;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: .4s;
}

button:hover {
  width: 170px;
  box-shadow: 0px 10px 10px rgba(0,0,0,0.4);
}

span, svg {
  position: absolute;
  color: #932e3e;
  fill: transparent;
  transition: .4s;
}

button:hover span {
  transition: .4s;
  font-size: 16px;
}

button:focus {
  outline: none;
  box-shadow: none;
  border: 2px solid transparent;
  width: 50px;
  border-left: 2px solid #932e3e;
  border-bottom: 2px solid #932e3e;
  animation: spin 2s 500ms forwards;
}

button:focus span {
  color: transparent;
}

button:focus svg {
  animation: check 500ms 2300ms forwards;
}

@keyframes spin {
  80% {
    border: 2px solid transparent;
    border-left: 2px solid #932e3e;
  }
  100% {
    transform: rotate(1080deg);
    border: 2px solid #932e3e;
  }
}

@keyframes check {
  to {
    fill: #932e3e;
  }
}

@keyframes circle {
  to {
    border: 2px solid #932e3e;
  }
}

