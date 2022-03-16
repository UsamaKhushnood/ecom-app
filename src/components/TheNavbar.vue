<template>
  <div>
    <b-navbar toggleable="lg" type="dark" variant="primary">
      <b-navbar-brand>
        <router-link to="/" tag="div"
          ><img
            src="@/assets/images/Logo.png"
            class=""
            width="90px"
            alt="s" /></router-link
      ></b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item>
            <router-link to="/contact" tag="span">Contact Us</router-link>
          </b-nav-item>
          <b-nav-item href="#">
            <router-link to="/about" tag="span">About Us</router-link>
          </b-nav-item>
          <b-nav-item href="#">
            <router-link to="/shop" tag="span">Shop</router-link>
          </b-nav-item>
        </b-navbar-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="ms-auto">
          <b-nav-form class="me-3">
            <b-form-input
              size="sm"
              class="me-sm-2"
              placeholder="Search"
            ></b-form-input>
            <b-button size="sm" class="my-2 my-sm-0" type="submit"
              >Search</b-button
            >
          </b-nav-form>

          <b-nav-item-dropdown text="Lang" right>
            <b-dropdown-item href="#">EN</b-dropdown-item>
            <b-dropdown-item href="#">ES</b-dropdown-item>
            <b-dropdown-item href="#">RU</b-dropdown-item>
            <b-dropdown-item href="#">FA</b-dropdown-item>
          </b-nav-item-dropdown>

          <b-nav-item-dropdown right>
            <!-- Using 'button-content' slot -->
            <template #button-content>
              <em>User</em>
            </template>
            <b-dropdown-item href="#">Profile</b-dropdown-item>
            <b-dropdown-item href="#">Sign Out</b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<style>
nav.navbar {
  padding: 10px 35px;
}
.form-inline {
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>
