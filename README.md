.hero {
  background: url('hero.jpg') center/cover no-repeat;
  height: 400px; /* un peu plus grand pour effet visuel */
  display: flex;
  align-items: center;
  justify-content: center;
  color: #fff;
  font-size: 2em;
  text-shadow: 2px 2px 8px rgba(0,0,0,0.7); /* rend le texte lisible */
  position: relative;
}

.hero::before {
  content: "";
  position: absolute;
  top: 0; left: 0;
  width: 100%; height: 100%;
  background: rgba(0,0,0,0.3); /* léger voile sombre pour le contraste */
  z-index: 0;
}

.hero > div {
  position: relative;
  z-index: 1
