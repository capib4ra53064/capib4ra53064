const state fps: 60,
};
color: "#0f0",
charset: "0123456789ABCDEF
size: 10
const gui= new datGui.GUI();
const fpsCtrl = gui.add(state, "fps").min(1).max(128).step(1); gui.addColor(state, "color");
gui.add(state, "charset");
const sizeCtrl = gui.add(state, "size").min(1).max(120).step(1);
const canvas = document.getElementById("canvas");
const ctx - canvas.getContext("2d");
let w, h, p;
const resize() => {
};
w - canvas.width
innerWidth;
h = canvas.height = innerHeight;
p = Array(Math.ceil(w/ state.size)).fill(0);
window.addEventListener("resize", resize); sizeCtrl.onFinishChange ((s) => resize())
resize();
