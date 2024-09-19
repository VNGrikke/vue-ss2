<template>
  <div>
    <h1>Danh sách khoá học</h1>
    <ul>
      <li>HTML</li>
      <li>CSS</li>
      <li>JAVASCRIPT</li>
      <li>REACTJS</li>
    </ul>

    <div class="flex-direction">
      <div class="red"></div>
      <div class="green"></div>
      <div class="blue"></div>
    </div>

    <div class="card">
      <div class="image">Image</div>
      <div>
        <p>Title</p>
        <button class="text-green-500">Add to card</button>
      </div>
    </div>

    <div>
      <div>{{ a }} + {{ b }} = {{ add(a, b) }}</div>
      <div>{{ a }} - {{ b }} = {{ subtract(a, b) }}</div>
      <div>{{ a }} * {{ b }} = {{ multiply(a, b) }}</div>
      <div>{{ a }} / {{ b }} = {{ divide(a, b) }}</div>
    </div>

    <div>
      <h1>Thông tin người dùng</h1>
      <ul>
        <li>Tên : {{ user.name }}</li>
        <li>Tuổi : {{ user.age }}</li>
        <li>Email : {{ user.email }}</li>
        <li>Ngày sinh : {{ user.dateOfBirth }}</li>
        <li>Địa chỉ : {{ user.address }}</li>
      </ul>
    </div>

    <div>
      <div>Ho va ten: {{ formatName(user2.firstName, user2.lastName) }}</div>
    </div>

    <div class="administrationPage">
      <div class="header">Header</div>
      <div class="body">
        <div class="menu">Menu</div>
        <div>
          <div class="main">main</div>
          <div class="footer">Footer</div>
        </div>
      </div>
    </div>
    <br>

    <div>
      <div class="header">header</div>
      <div class="body">
        <div class="menu">menu</div>
        <div class="listCart">
          <div>cart</div>
          <div>cart</div>
          <div>cart</div>
          <div>cart</div>
          <div>cart</div>
          <div>cart</div>
          <div>cart</div>
          <div>cart</div>
          <div>cart</div>
          <div>cart</div>
          <div>cart</div>
          <div>cart</div>
          <div>cart</div>
          <div>cart</div>
          <div>cart</div>
          <div>cart</div>
        </div>
        <div class="menu">article</div>
      </div>
    </div>
    <B9/>
    <br>
    <B10/>
  </div>
</template>

<script setup>
import B9 from './components/b9.vue';
import B10 from './components/b10.vue';

const a = 5;
const b = 10;

const add = (a, b) => a + b;
const multiply = (a, b) => a * b;
const subtract = (a, b) => a - b;
const divide = (a, b) => a / b;

const user = {
  name: "John Doe",
  age: 30,
  email: "john.doe@example.com",
  address: "123 Main St, City, State, ZIP",
  dateOfBirth: "15/11/2005",
};
const user2 = {
  firstName: "Vuong",
  lastName: "Nguyen",
};
const formatName = (a, b) => {
  let name = b + " " + a;
  return name;
};
</script>

<style>
.flex-direction {
  display: flex;
  gap: 10px;
}

.red {
  width: 100px;
  height: 100px;
  background-color: red;
}
.blue {
  width: 100px;
  height: 100px;
  background-color: blue;
}
.green {
  width: 100px;
  height: 100px;
  background-color: green;
}

.card {
  height: 150px;
  width: 100px;
  border-radius: 10px;
  align-items: center;
  border: 1px solid black;
}

.image {
  background-color: grey;
  height: 70px;
  text-align: center;
  line-height: 70px;
  border-top-left-radius: 10px;
  border-top-right-radius: 10px;
}

.header {
  background-color: bisque;
  text-align: center;
  height: 5vh;
}
.body {
  display: flex;
}
.menu {
  width: 200px;
  background-color: lightblue;
  text-align: center;
  height: 70vh;
}
.main {
  flex: 1;
  background-color: lightgreen;
  height: 65vh;
  width: 158vh;
}
.footer {
  background-color: rgb(255, 255, 0);
  text-align: center;
  height: 5vh;
}
.listCart{
  display: flex;
  flex-wrap: wrap;
  gap: 10px;

}

.listCart> div {
  flex-basis: calc(25% - 10px);
  box-sizing: border-box; 
  width: 60px;
  height: 60;
  background-color: lightgray;
  text-align: center;
}
</style>
