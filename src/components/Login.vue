<template>
  <div class="container-login-form">
    <div class="image-container">
      <img
        src="https://diginet.com.vn/wp-content/uploads/2020/10/tai-sao-task-management-lai-quan-trong-voi-doanh-nghiep-1.png"
        alt="Italian Trulli"
      />
    </div>
    <div class="form-container">
      <h1>Logo</h1>
      <h1>welcome back</h1>
      <form class="login-form">
        <div class="form-control">
          <label>Account</label>
          <input type="text" id="username" placeholder="Username" />
          <small></small>
        </div>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: "LoginFrom",
  setup() {},
};
</script>

<style>
.container-login-form {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 400px;
  border-radius: 10px;
  box-shadow: 0px 0px 15px rgba(0, 0, 0, 0.05);
}

@media screen and (max-width: 720px) {
  .container-login-form {
    position: absolute;
    display: flex;
    flex-direction: column;
    height: 100vh;
    width: 100vw;
  }

  .image-container {
    justify-content: center;
    align-items: center;
    overflow: hidden;
    height: 30vh;
    width: auto;
  }

  .image-container img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }

  .form-container {
    justify-content: center;
    flex-direction: column;
    align-items: flex-start;
  }

  .form-container span,
  input {
    display: inline-block;
  }

  .form-control {
    width: 100%;
  }
}
</style>