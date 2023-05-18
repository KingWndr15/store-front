<template>
  <footer>
      <section>
        <div class="footer-categories">
          <div class="product-categories">
            <h2>Categories</h2>
            <ul>T-Shirts</ul>
            <ul>Hoodies</ul>
            <ul>Accesories</ul>
          </div>

        <div class="trending-collections">
          <h2>Collections</h2>
          <ul>New In</ul>
          <ul>Throwback</ul>
        </div>
        </div>

        <form>
          <h2>Language & Currency</h2>
          <select>
            <option value="english">English</option>
          </select>
          <select>
            <option value="GBP">GBP</option>
          </select>
        </form>
      </section>

      <div class="bottom">
        <p>© 2023 GraphCMS GmbH. All rights reserved.</p>
        <div class="icons">
          <img src="@/assets/images/twitter-icon.svg" alt="">
          <img src="@/assets/images/github-icon.svg" alt="">
        </div>
      </div>
  </footer>

</template>

<script>

export default {
  name: 'App',
  components: {}
}
</script>

<style>
@import '@/assets/css/main.css';
@import '@/assets/css/variable.css';

#app {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}

footer {
  width: 80%;
  margin: 64px 0px 0px 0px;  
}

footer section {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  flex-wrap: wrap;
  width: 100%;
  margin-bottom: 76px;
}

footer section .footer-categories {
  display: flex;
  justify-content: center;
}

footer section .footer-categories div {
  display: flex;
  flex-direction: column;
  gap: 15px;
  padding: 0px 50px 0px 0px;
}

footer section .footer-categories div ul {
  cursor: pointer;
}

footer section form {
  display: flex;
  flex-direction: column;
  gap: 15px;
}

footer section form select {
  padding: 8px 18px 8px 13px;
  border: 1px solid #D1D5DB;
  outline: none;
  border-radius: 6px;
}

footer .bottom {
  width: 100%;
  display: flex;
  align-items: flex-end;
  justify-content: space-between;
  border-top: 1px solid #E5E7EB;
  flex-wrap: wrap;
  padding: 33px 0px 0px;
}

footer .bottom p {
  color: #9CA3AF !important;
  margin: 0px 33.5px 0px 0px ;
}

footer .icons {
  padding: 0px 0px 0px 10px;
  display: flex;
  gap: 28px;
}

@media (max-width: 538px) {
  footer section form {
    margin: 25px 0px 0px;
  }
}

@media (max-width: 549px) {
  footer .icons {
    margin-top: 20px;
  }
} 
</style>
