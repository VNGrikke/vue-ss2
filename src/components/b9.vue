<template>
  <div>
    <table>
      <thead>
        <tr>
          <th>STT</th>
          <th>Tên</th>
          <th>Ngày sinh</th>
          <th>Giới tính</th>
          <th>Địa chỉ</th>
          <th>Hành động</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(item, index) in students" :key="item.id">
          <td>{{ index + 1 }}</td>
          <td>{{ item.name }}</td>
          <td>{{ item.dob }}</td>
          <td>{{ item.gender }}</td>
          <td>{{ item.address }}</td>
          <td>
            <button>Xóa</button>
            <button>Sửa</button>
          </td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script setup>
const students = [
  {
    id: 1,
    name: "John Doe",
    dob: "1990-05-15",
    gender: "Nam",
    address: "123 Main St",
  },
  {
    id: 2,
    name: "Jane Smith",
    dob: "1985-12-25",
    gender: "Nữ",
    address: "456 Elm St",
  },
];
</script>

<style>
</style>