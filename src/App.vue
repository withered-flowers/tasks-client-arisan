<script>
export default {
  name: 'App'
}
</script>

<template>
  <!-- Login Section -->
  <section
    class="p-4 min-w-full min-h-screen bg-gray-100 flex items-center justify-center border-red-100 border text-slate-700"
  >
    <form>
      <h1 class="text-3xl font-semibold mb-4 text-center">Login Arisan</h1>
      <form>
        <section class="flex flex-col gap-2">
          <input
            class="px-4 py-2 rounded hover:ring-2 hover:ring-blue-100 transition-all duration-200"
            type="text"
            placeholder="Username"
          />
          <input
            class="px-4 py-2 rounded hover:ring-2 hover:ring-blue-100 transition-all duration-200"
            type="password"
            placeholder="Password"
          />
          <button
            class="px-4 py-2 rounded bg-blue-200 hover:bg-blue-400 hover:text-white transition-colors duration-300"
          >
            Login
          </button>
        </section>
      </form>
    </form>
  </section>

  <!-- Club List Section -->
  <section class="p-4 min-w-full min-h-screen bg-gray-100 border border-green-100 text-slate-700">
    <section class="flex justify-between items-center">
      <div class="left">
        <h2 class="text-2xl font-semibold">List Club</h2>
      </div>
      <div class="right flex gap-2">
        <p>Welcome, {username}</p>
        <p>Your Balance is: {saldo}</p>

        <a
          href="#"
          class="underline text-blue-600 hover:text-red-600 transition-colors duration-300"
          >Log Out</a
        >
      </div>
    </section>

    <table class="table-auto border-collapse border border-slate-400">
      <thead>
        <tr>
          <th class="border border-emerald-500 px-4 py-2">Id</th>
          <th class="border border-emerald-500 px-4 py-2">Nama Club</th>
          <th class="border border-emerald-500 px-4 py-2">Pool Uang Arisan</th>
          <th class="border border-emerald-500 px-4 py-2">Action</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td class="border border-emerald-500 py-2 text-center">1</td>
          <td class="border border-emerald-500 py-2 text-center">Lorem Ipsum</td>
          <td class="border border-emerald-500 py-2 text-center">Rp 150.000.000,00</td>
          <td class="border border-emerald-500 text-center">
            <!-- Initial Button on Table -->
            <div>
              <button
                class="px-4 py-2 rounded bg-blue-200 hover:bg-blue-400 hover:text-white transition-colors duration-300"
              >
                Add Pool
              </button>
            </div>

            <!-- If Add Pool is Clicked -->
            <div class="flex gap-2">
              <input type="number" class="py-2 px-4" placeholder="Amount" />
              <button
                class="px-4 py-2 rounded bg-blue-200 hover:bg-blue-400 hover:text-white transition-colors duration-300"
              >
                Add
              </button>
            </div>
          </td>
        </tr>
      </tbody>
    </table>
  </section>

  <!-- Gift List Section -->
  <section class="p-4 min-w-full min-h-screen bg-gray-100 border border-blue-100 text-slate-700">
    <h2 class="text-2xl font-semibold">List Gift</h2>
  </section>
</template>
