<template>
  <div class="max-w-sm m-auto my-8">
    <div class="border p-10 border-grey-200 hadow rounded">
      <h3 class="text-2xl mb-6 text-grey-900">Sign Up</h3>
      <form @submit.prevent="signup">
        <div class="text-red" v-if="error">{{ error }}</div>

        <div class="mb-6">
          <label for="email" class="label">E-mail Address</label>
          <input type="email" v-model="email" class="input" id="email" placeholder="pedro@gmail.com">
        </div>

        <div class="mb-6">
          <label for="password" class="label">Password</label>
          <input type="password" v-model="password" class="input" id="password" placeholder="Password">
        </div>
        <div class="mb-6">
          <label for="password_confirmation" class="label">Password Confirmation</label>
          <input type="password" v-model="password_confirmation" class="input" id="password_confirmation" placeholder="Password confirmation">
        </div>
        <button type="submit" class="font-sans rounded bg-green-400 font-bold px-4 cursor-pointer hover:bg-green-600 w-full py-4 text-white block items-center justify-center">Sign Up</button>

        <div class="my-4"><router-link to="/" class="text-gray-500">Sing In</router-link></div>
      </form>
    </div>
  </div>

</template>

<script>
export default {
  
}
</script>
