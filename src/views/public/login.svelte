<script>
  import Card from "../../components/Cards/Card.svelte";
  import BaseButton from "../../components/BaseButton.svelte";
  import BaseInput from "../../components/Inputs/BaseInput.svelte";
  import BaseCheckbox from "../../components/Inputs/BaseCheckbox.svelte";
  document.body.classList = "bg-default";
  import { fade, scale } from "svelte/transition";
</script>

<div in:scale={{ y: 200, duration: 500 }} out:scale={{ y: 200, duration: 100 }}>
  <div class="header bg-gradient-danger py-7 py-lg-8 pt-lg-9">
    <div class="container">
      <div class="header-body text-center mb-7">
        <div class="row justify-content-center">
          <div class="px-5 col-md-8 col-lg-6 col-xl-5">
            <h1 class="text-white">Welcome!</h1>
            <p class="text-lead text-white">
              Use these awesome forms to login or create new account in your
              project for free.
            </p>
          </div>
        </div>
      </div>
    </div>
    <div class="separator separator-bottom separator-skew zindex-100">
      <svg
        x="0"
        y="0"
        viewBox="0 0 2560 100"
        preserveAspectRatio="none"
        version="1.1"
        xmlns="http://www.w3.org/2000/svg">
        <polygon points="2560 0 2560 100 0 100" class="fill-default" />
      </svg>
    </div>
  </div>
  <div class="mt--8 pb-5 container">
    <div class="row justify-content-center">
      <div class="col-md-7 col-lg-5">
        <Card
          noBody
          className="bg-secondary border-0 mb-0 card"
          headerClasses="bg-transparent pb-5"
          bodyClasses="px-lg-5 py-lg-5">
          <div slot="header">
            <div class="text-muted text-center mt-2 mb-3">
              <small>Sign in with</small>
            </div>
            <div class="btn-wrapper text-center">
              <a href="/login/github" class="btn btn-neutral btn-icon">
                <span class="btn-inner--icon">
                  <img src="img/icons/common/github.svg" alt="" />
                </span>
                <span class="btn-inner--text">Github</span>
              </a>
              <a href="/login/google" class="btn btn-neutral btn-icon">
                <span class="btn-inner--icon">
                  <img src="img/icons/common/google.svg" alt="" />
                </span>
                <span class="btn-inner--text">Google</span>
              </a>
            </div>
          </div>
        </Card>
      </div>
    </div>
  </div>
</div>
