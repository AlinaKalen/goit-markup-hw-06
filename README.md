# goit-markup-hw-06









.page-header .container {
  min-height: 80px;
  display: flex;
  align-items: center;
  justify-content: flex-end;
}

.menu {
  display: flex;
  padding: 0;
  margin: 0;
  list-style: none;
}

@media (max-width: 767px) {
  .menu {
    display: none;
  }
}

.menu .link {
  padding: 10px;
  color: inherit;
  text-decoration: none;
}

.menu .link:hover,
.menu .link:focus {
  text-decoration: underline;
}

.menu-toggle {
  min-height: 40px;
  min-width: 40px;
  display: flex;
  align-items: center;
  justify-content: center;

  margin: 0;
  padding: 0;
  background-color: transparent;
  cursor: pointer;
  border: none;
  border-radius: 50%;
  outline: none;
}

@media (min-width: 768px) {
  .menu-toggle {
    display: none;
  }
}

.menu-toggle:hover,
.menu-toggle:focus {
  background-color: rgba(0, 0, 0, 0.1);
}

.menu-container {
  position: fixed;
  top: 0;
  left: 0;
  width: 100vw;
  height: 100vh;
  padding: 32px;
  background-color: #3f51b5;
  z-index: 999;

  transform: translateX(100%);
  transition: transform 250ms ease-in-out;
}

.menu-container.is-open {
  transform: translateX(0);
}

.menu-container .menu-toggle {
  position: absolute;
  top: 16px;
  right: 16px;
  color: #fff;
}

.mobile-menu {
  padding: 0;
  margin: 0;
  list-style: none;
}

.mobile-menu .link {
  display: block;
  padding: 10px;
  color: #fff;
  text-decoration: none;
}
