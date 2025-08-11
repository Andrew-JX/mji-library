<!-- src/components/Form.vue -->
<template>
  <div class="container mt-5">
    <div class="row">
      <div class=col-md-8 offset-md-2>
        <h1>User Information Form</h1>
        <form @submit.prevent="submitForm">
          <div class="mb-3">
            <div class="col-md-6">
              <label for="username" class="form-label">Username:</label>
              <input type="text" id="username" name="username" class="form-control" v-model="formData.username"
                required>
            </div>
            <div class="col-md-6">
              <label for="password" class="form-label">Password:</label>
              <input type="password" id="password" name="password" class="form-control" v-model="formData.password"
                required>
            </div>

            <div class="mb-3 form-check">
              <input type="checkbox" id="isAustralian" name="isAustralian" class="form-check-input"
                v-model="formData.isAustralian">
              <label for="isAustralian" class="form-check-label">Australian Resident?</label>
            </div>

            <div class="mb-3">
              <label for="reason" class="form-label">Reason For Joining:</label>
              <textarea id="reason" name="reason" rows="3" class="form-control" v-model="formData.reason"></textarea>
            </div>

            <div class="mb-3">

              <div class="col-md-6 offset-md-3">
                <h2 class="text-center">User Information Form</h2>
              </div>

              <form>
                <label for="username">Username:</label><br>
                <input type="text" id="username" name="username"><br>

                <label for="password">Password:</label><br>
                <input type="password" id="password" name="password"><br>

                <label for="isAustralian">Australian Resident?</label><br>
                <input type="checkbox" id="isAustralian" name="isAustralian"><br>

                <label for="reason">Reason For Joining:</label><br>
                <textarea id="reason" name="reason" rows="3"></textarea><br>

                <label for="gender">Gender</label><br>
                <select id="gender">
                  <option value="female">Female</option>
                  <option value="male">Male</option>
                  <option value="other">Other</option>
                </select>
              </form>
            </div>
</template>

<script setup>

</script>

<style scoped></style>