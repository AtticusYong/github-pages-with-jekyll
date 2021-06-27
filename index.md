---
title: "Welcome to My Website"
---

Hello I am Atticus Yong. I like coding a lot. I also like to play chess. I play badminton too. I am quite good at chess. I also like exercising. I am ten years old and my birthday is coming later this year on **/**/****. Here is some code that I did: index.html ->
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>Three.js app</title>
    <link href="style.css" rel="stylesheet" type="text/css" />
  </head>
  <body>
    <canvas id = "bg"></canvas>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/104/three.min.js"></script>
    <script src="https://unpkg.com/three@0.85.0/examples/js/controls/OrbitControls.js"></script>

       <!-- <main>

      <header>
        <h1>Jeff Delaney</h1>
        <p>🚀 Welcome to my website!</p>
      </header>


      <blockquote>
        <p>I like making stuff and putting it on the internet</p>
      </blockquote>

      <section>
        <h2>📜 Manifesto</h2>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>

        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>

        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>

      </section>

      <section class="light">
        <h2>👩🏽‍🚀 Projects</h2>

        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>

        <h2>🏆 Accomplishments</h2>

        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>

      </section>

      <blockquote>
        <p>The best way out is always through <br>-Robert Frost</p>
      </blockquote>

      <section class="left">
        <h2>🌮 Work History</h2>

        <h3>McDonalds</h3>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>
        <h3>Burger King</h3>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>
        <h3>Taco Bell</h3>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>

      </section>

      <blockquote>
        <p>Thanks for watching!</p>
      </blockquote>


    </main> -->

    <script src="script.js"></script>
  </body>
</html>

script.js ->

// import MathUtils from './MathUtils'

const scene = new THREE.Scene()
const camera = new THREE.PerspectiveCamera( 75, window.innerWidth / window.innerHeight, 0.1, 1000 );
const renderer = new THREE.WebGLRenderer({
  canvas: document.querySelector('#bg'),
});
renderer.setPixelRatio(window.devicePixelRatio);
renderer.setSize(window.innerWidth, window.innerHeight);
camera.position.setZ(30);

renderer.render(scene, camera);

function moveCamera() {
  const t = document.body.getBoundingClientRect().top;
  moon.rotation.x += 0.05;
  moon.rotation.y += 0.075;
  moon.rotation.z += 0.05;

  jeff.rotation.y += 0.01;
  jeff.rotation.z += 0.01;

  camera.position.z = t * -0.01;
  camera.position.x= t * -0.0002;
  camera.position.y = t * -0.0002;
}

document.body.onscroll = moveCamera

// const geometry = new THREE.TorusGeometry(10, 3, 16, 100);
// const material = new THREE.MeshStandardMaterial({ color: 0x2874 });
// const torus = new THREE.Mesh(geometry, material);

// scene.add(torus)

const pointLight = new THREE.PointLight(0xffffff)
pointLight.position.set(5, 5, 5)

const ambientLight = new THREE.AmbientLight(0xffffff);
scene.add(pointLight, ambientLight)

const lightHelper = new THREE.PointLightHelper(pointLight)
// const gridHelper = new THREE.GridHelper(10000, 2500);
scene.add(lightHelper,)

const controls = new THREE.OrbitControls(camera, renderer.domElement);

// Avatar 

const galaxyTexture = new THREE.TextureLoader().load('cool-galaxy.jpg');

const galaxy = new THREE.Mesh(
  new THREE.BoxGeometry(3, 3, 3),
  new THREE.MeshBasicMaterial({map: galaxyTexture})
);

scene.add(galaxy);

// Solar System

const sunTexture = new THREE.TextureLoader().load('sun.jpg');

const sun = new THREE.Mesh(
  new THREE.SphereGeometry(8, 60, 60),
  new THREE.MeshBasicMaterial({
    map: sunTexture
    })
);

scene.add(sun)

const mercuryTexture = new THREE.TextureLoader().load('mercury.jpeg');

const mercury = new THREE.Mesh(
  new THREE.SphereGeometry(2, 20,20),
  new THREE.MeshBasicMaterial({
    map: mercuryTexture
    })
);

scene.add(mercury)

mercury.position.z = 0;
mercury.position.setX(-20);

const venusTexture = new THREE.TextureLoader().load('venus.jpg');

const venus = new THREE.Mesh(
  new THREE.SphereGeometry(2, 33, 33),
  new THREE.MeshBasicMaterial({
    map: venusTexture
    })
);

scene.add(venus)

venus.position.z = 0;
venus.position.setX(-40);


const earthTexture = new THREE.TextureLoader().load('earth.jpg');

const earth = new THREE.Mesh(
  new THREE.SphereGeometry(3, 33, 33),
  new THREE.MeshBasicMaterial({
    map: earthTexture
    })
);

scene.add(earth)

earth.position.z = 0;
earth.position.setX(-60);

const moonTexture = new THREE.TextureLoader().load('moon.jpg');
const normalTexture = new THREE.TextureLoader().load('normal.jpg');

const moon = new THREE.Mesh(
  new THREE.SphereGeometry(2, 15, 15),
  new THREE.MeshBasicMaterial({
    map: moonTexture,
    normalMap: normalTexture
    })
);

scene.add(moon)

moon.position.z = 0;
moon.position.setX(-67);

const marsTexture = new THREE.TextureLoader().load('mars.jpeg');

const mars = new THREE.Mesh(
  new THREE.SphereGeometry(2.5, 26, 26),
  new THREE.MeshBasicMaterial({
    map: marsTexture
    })
);

scene.add(mars)

mars.position.z = 0;
mars.position.setX(-80);


const jupiterTexture = new THREE.TextureLoader().load('jupiter.jpg');

const jupiter = new THREE.Mesh(
  new THREE.SphereGeometry(6, 50, 50),
  new THREE.MeshBasicMaterial({
    map: jupiterTexture
    })
);

scene.add(jupiter)

jupiter.position.z = 0;
jupiter.position.setX(-100);


const saturnTexture = new THREE.TextureLoader().load('saturn.jpg');

const saturn = new THREE.Mesh(
  new THREE.SphereGeometry(5, 45, 45),
  new THREE.MeshBasicMaterial({
    map: saturnTexture
    })
);

scene.add(saturn)

saturn.position.z = 0;
saturn.position.setX(-120);

// const saturnringsTexture = new THREE.TextureLoader().load('saturnrings.jpg');

// const saturnrings = new THREE.Mesh(
//   new THREE.CircleGeometry(60, 60),
//   new THREE.MeshBasicMaterial({
//     map: saturnringsTexture
//     })
// );

// scene.add(saturnrings)

// saturnrings.position.z = 100;
// saturnrings.position.setX(-120);


// const circle = {
//   // The geometry: the shape & size of the object
//   geometry: new THREE.CircleGeometry(5, 60),
//   // The material: the appearance (color, texture) of the object
//   material: new THREE.MeshBasicMaterial({ color: 0xff8000 })
// };

// const geometry = new THREE.CircleGeometry( 60, 60 );
// const material = new THREE.MeshBasicMaterial( { color: #BD650C } );
// const circle = new THREE.Mesh( geometry, material );
// circle.position.z = 100;
// circle.position.setX(-120);

// scene.add(circle);

const uranusTexture = new THREE.TextureLoader().load('uranus.jpg');

const uranus = new THREE.Mesh(
  new THREE.SphereGeometry(5, 45, 45),
  new THREE.MeshBasicMaterial({
    map: uranusTexture
    })
);

scene.add(uranus)

uranus.position.z = 0;
uranus.position.setX(-140);

const neptuneTexture = new THREE.TextureLoader().load('neptune.jpg');

const neptune = new THREE.Mesh(
  new THREE.SphereGeometry(5, 45, 45),
  new THREE.MeshBasicMaterial({
    map: neptuneTexture
    })
);

scene.add(neptune)

neptune.position.z = 0;
neptune.position.setX(-160);


function addStar() {
  const geometry = new THREE.SphereGeometry(0.25, 24, 24);
  const material = new THREE.MeshStandardMaterial({color: 0xffffff})
  const star = new THREE.Mesh(geometry, material);

  const [x, y, z] = Array(3).fill().map(() => 500 * Math.random() - 100);

  star.position.set(x, y, z);
  scene.add(star)

}

  Array(500).fill().forEach(addStar)

  const spaceTexture = new THREE.TextureLoader().load('space.jpg');
  scene.background = spaceTexture;

function animate() {
  requestAnimationFrame(animate)

  // torus.rotation.x += 0.01;
  // torus.rotation.y += 0.005;
  // torus.rotation.z += 0.01;

  controls.update();

  renderer.render(scene, camera);
}

animate();

style.css -> 

canvas {
  position: fixed;
  top: 0;
  left: 0;
}

main {
  position: absolute;
}
