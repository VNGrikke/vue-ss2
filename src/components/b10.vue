<template>
  <div class="container py-5 h-100">
    <div class="row d-flex justify-content-center align-items-center h-100">
      <div class="col col-xl-10">
        <div class="card2">
          <div class="card2-body p-5">
            <h3 class="text-center mb-4">Quản lý công việc</h3>

            <form class="d-flex justify-content-center align-items-center mb-4">
              <div class="form-outline flex-fill">
                <input
                  type="text"
                  id="form2"
                  class="form-control"
                  placeholder="Thêm công việc"
                />
                <button type="submit" class="btn btn-info ms-2">Thêm</button>
              </div>
            </form>

            <ul class="nav nav-tabs mb-4 pb-2" id="ex1" role="tablist">
              <li class="nav-item" role="presentation">
                <a class="nav-link active">Tất cả công việc</a>
              </li>
            </ul>

            <div class="tab-content">
              <div class="tab-pane fade show active">
                <ul class="list-group mb-0">
                  <li
                    class="list-group-item d-flex align-items-center border-0 mb-2 rounded justify-content-between"
                  >
                    <div>
                      <input
                        class="form-check-input me-2"
                        type="checkbox"
                        checked
                      />
                      <s>Cras justo odio</s>
                    </div>
                    <div>
                      <a href="#!" class="text-info" title="Sửa công việc">
                        <i class="fas fa-pencil-alt me-3"></i>
                      </a>
                      <a href="#!" class="text-danger" title="Xóa công việc">
                        <i class="fas fa-trash-alt"></i>
                      </a>
                    </div>
                  </li>
                  <li
                    class="list-group-item d-flex align-items-center border-0 mb-2 justify-content-between"
                  >
                    <div>
                      <input class="form-check-input me-2" type="checkbox" />
                      Cras justo odio
                    </div>
                    <div>
                      <a href="#!" class="text-info" title="Sửa công việc">
                        <i class="fas fa-pencil-alt me-3"></i>
                      </a>
                      <a href="#!" class="text-danger" title="Xóa công việc">
                        <i class="fas fa-trash-alt"></i>
                      </a>
                    </div>
                  </li>
                </ul>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Roboto", sans-serif;
}

body {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
  background-color: #f7f7f7;
}

.container {
  width: 100%;
  max-width: 800px;
}

.card2 {
  border-radius: 10px;
  box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.1);
  background-color: white;
  padding: 30px;
}

h3 {
  text-align: center;
  color: #333;
  margin-bottom: 20px; 
}

.form-control {
  border: 1px solid #d3d3d3;
  padding: 10px;
  border-radius: 5px;
  font-size: 16px;
  width: calc(100% - 120px); 
}

button {
  background-color: #17a2b8;
  color: white;
  border: none;
  padding: 10px 15px;
  border-radius: 5px;
  font-size: 16px; 
  cursor: pointer;
  transition: background-color 0.3s ease;
}

button:hover {
  background-color: #138496;
}

.nav-tabs {
    margin-top: 20px;
    margin-bottom: 20px;
    list-style-type: none;
}

.nav-link {
  font-size: 16px;
  color: #007bff;
  padding: 8px 15px;
  cursor: pointer;
}

.nav-link.active {
  font-weight: 500;
  border-bottom: 2px solid #007bff;
  color: #007bff;
}

.list-group {
  list-style-type: none; /* Removes bullets from the list */
  padding: 0;
}

.list-group-item {
  display: flex;
  align-items: center;
  justify-content: space-between;
  background-color: #f8f9fa;
  border: none;
  padding: 15px 20px;
  border-radius: 5px;
  margin-bottom: 10px;
}

.list-group-item input[type="checkbox"] {
  margin-right: 10px;
}

.list-group-item s {
  color: #888;
}

.text-info {
  color: #17a2b8;
  margin-right: 10px;
}

.text-info:hover {
  color: #138496;
}

.text-danger {
  color: #dc3545;
}

.text-danger:hover {
  color: #c82333;
}
</style>
