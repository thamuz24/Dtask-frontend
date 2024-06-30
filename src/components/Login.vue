<template>
  <div class="container-login-form">
    <div class="image-container">
      <img
        src="https://diginet.com.vn/wp-content/uploads/2020/10/tai-sao-task-management-lai-quan-trong-voi-doanh-nghiep-1.png"
        alt="Italian Trulli"
      />
    </div>
    <div class="form-container">
      <h1 class="wellcome">Dtask xin chào</h1>
      <form class="login-form">
        <div class="form-control">
          <label class="form-control-item">Tài khoản</label>
          <input
            class="form-control-item"
            type="text"
            id="username"
            placeholder="Tài khoản"
          />
          <small></small>
        </div>

        <div class="form-control">
          <label class="form-control-item">Mật khẩu</label>
          <input
            class="form-control-item password"
            id="password"
            placeholder="Mật khẩu"
          />
          <small></small>
        </div>

        <div class="from-control">
          <button class="login-button">Đăng nhập</button>
          <p>Bạn chưa có tài khoản?</p>
          <a href="http://webcoban.vn">Đăng ký tại đây</a>
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
.wellcome {
  margin-top: 20px;
  font-size: 40px;
}

.container-login-form {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 400px;
  border-radius: 10px;
  box-shadow: 0px 0px 15px rgba(0, 0, 0, 0.05);
}

.form-control {
  margin-top: 30px;
}

.form-control-item {
  display: inline-block;
  width: 100%;
  height: 50px;
  text-align: left;
  font-size: 30px;
}

input {
  padding-left: 20px;
  border-radius: 10px;
  color: white;
  background-color: #1d212f;
  border: 4px solid #4c416c;
  transition: box-shadow 0.3s ease;
}

input:focus {
  outline: none;
  box-shadow: 0 0 8px #cfc2f5;
  border: 4px solid #9580c4;
}

input:-webkit-autofill,
input:-webkit-autofill:hover,
input:-webkit-autofill:focus,
input:-webkit-autofill:active {
  -webkit-box-shadow: 0 0 0 30px #1d212f inset !important;
  -webkit-text-fill-color: #ffffff !important;
}

input::placeholder {
  color: #6a6969;
  transition: color 0.3s ease;
}

input:focus::placeholder {
  color: #9580c4;
}

.login-button {
  width: 100%;
  height: 40px;
  margin-top: 30px;
  border-radius: 10px;
  border: none;
  background: linear-gradient(to right, #7168b0, #94b9d4);
}

a {
  text-decoration: none;
  color: #cfc2f5;
}
a,
p {
  display: inline-block;
  margin-right: 10px; /* Thêm khoảng cách giữa các phần tử */
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
    position: relative;
    width: 80%;
    left: 10%;
  }

  .form-control-item {
    display: inline-block;
    width: 100%;
    height: 40px;
    text-align: left;
    font-size: 20px;
  }
}
</style>