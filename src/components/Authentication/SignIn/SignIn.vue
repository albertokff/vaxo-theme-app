<template>
  <div class="h-80vh">
    <div class="d-table">
      <div class="d-table-cell">
        <div
          class="card border-0 box-shadow border-radius-10 mb-4 w-100"
          style="max-width: 500px; margin: auto"
        >
          <div class="card-body p-30">
            <div class="text-center mb-4">
              <h4 class="fs-20 fw-semibold mb-2">Sign In</h4>
              <p class="fs-14 text-body">
                Don’t have an account yet?
                <router-link
                  to="/sign-up"
                  class="text-primary text-decoration-none"
                >
                  Sign Up
                </router-link>
              </p>
            </div>
            <form>
              <div class="form-group mb-4">
                <label class="label">Email Address</label>
                <input
                  type="text"
                  class="form-control"
                  placeholder="example@gmail.com"
                />
              </div>
              <div class="form-group mb-4">
                <label class="label">Your Password</label>
                <div class="password-wrapper position-relative">
                  <input
                    type="password"
                    id="password"
                    class="form-control"
                    value="password"
                  />
                  <i
                    style="
                      color: #919aa3;
                      font-size: 16px;
                      right: 15px !important;
                    "
                    class="ri-eye-off-line password-toggle-icon translate-middle-y top-50 end-0 position-absolute"
                    aria-hidden="true"
                  ></i>
                </div>
              </div>
              <div class="form-group mb-4 d-flex justify-content-between">
                <div class="c-form-check form-check">
                  <input
                    class="form-check-input"
                    type="checkbox"
                    value=""
                    id="flexCheckDefault"
                  />
                  <label
                    class="form-check-label fs-14 text-body ms-0"
                    for="flexCheckDefault"
                  >
                    Remember me
                  </label>
                </div>
                <router-link
                  to="/forget-password"
                  class="text-primary fs-14 text-decoration-none"
                >
                  Forget you password?
                </router-link>
              </div>
              <div class="form-group mb-4">
                <button type="submit" class="default-btn w-100 d-block">
                  Sign In
                </button>
              </div>
              <div class="form-group mb-4">
                <span class="or text-center d-block">
                  <span class="fs-18 fw-medium text-dark">OR</span>
                </span>
              </div>
              <div class="form-group mb-0">
                <button
                  type="submit"
                  class="default-btn w-100 d-block"
                  style="background-color: #dd4b39"
                >
                  <i class="ri-google-fill"></i> Sign in with Google
                </button>
              </div>
            </form>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SignIn",
};
</script>