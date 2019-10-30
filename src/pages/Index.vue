<template>
  <Layout>
    <img class="greet-image" src="../assets/images/1x/logo_white.png" />

    <h2 class="mb-2 font-weight-lighter text-white text-center">COME TO US WITH A VISION. WE’LL HELP YOU CRAFT IT.</h2>
    <h5 class="font-weight-normal text-gray pt-2  text-center">We build digital product, from idea to design, development to marketing & PR to post launch support</h5>
    <button type="button" class="btn btn-primary mt-3 btn-block">Get Free Consultation</button>

    <div class="box">
      <span class="oi oi-browser"></span>
      <h4 class="mt-4">Domains</h4>
      <p>
        You can’t have a website without a domain name. Like a street address that tells people where you live, a domain helps customers drive directly to your website. We can help you find one you’ll love.
      </p>
    </div>
    <div class="box">
      <span class="oi oi-monitor"></span>
      <h4 class="mt-4">Hosting</h4>
      <p>
        Hosting is what makes your site visible on the web. We offer fast, reliable plans for every need - from a basic blog to high-powered site. Designer? Developer? We've got you covered too.
      </p>
    </div>
    <div class="box">
      <span class="oi oi-person"></span>
      <h4 class="mt-4">Support</h4>
      <p>
        We're here with the help and advice you need to bring your idea to life. When you're ready to get online, we're prepped, trained, and ready to guide you from start to success.
      </p>
    </div>

  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Kosowwwa LLC'
  }
}
</script>

<style lang="scss">
.greet-image {
  display: block;
  margin: auto;
  width: 100%;
  max-width: 500px;
  padding: 0 0 50px 0;
}
.box {
    border: 1px solid #000;
    margin: 1.5rem 0;
    padding: 20px;
    background-color: #060606;
    box-shadow: 0 1px 2px rgba(0,0,0,0.07), 0 2px 4px rgba(0,0,0,0.07), 0 4px 8px rgba(0,0,0,0.07), 0 8px 16px rgba(0,0,0,0.07), 0 16px 32px rgba(0,0,0,0.07), 0 32px 64px rgba(0,0,0,0.07);
    color: #cccccc;
    span {
      font-size: 1.5rem;
    }
    h4 {
      color: #d1a74f;
    }
}
.howWeWork {
  img {
    width: 50%;
    display: block;
    margin: auto;
  }
}
</style>
