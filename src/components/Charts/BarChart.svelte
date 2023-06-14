<script>
  let isOn = false;

  const updateBarChart = on => {
    
  };
</script>

<div class="col-span-2 bg-white rounded-md dark:bg-darker">
  <!-- Card header -->
  <div
    class="flex items-center justify-between p-4 border-b dark:border-primary"
  >
    <h4 class="text-lg font-semibold text-gray-500 dark:text-light">
      Login Button
    </h4>
    <div class="flex items-center space-x-2">
      <span class="text-sm text-gray-500 dark:text-light">Last year</span>
      <button
        class="relative focus:outline-none"
        on:click={() => {
          isOn = !isOn;
          updateBarChart(isOn);
        }}
      >
        <div
          class="w-12 h-6 transition rounded-full outline-none bg-primary-100 dark:bg-primary-darker"
        />
        <div
          class="{isOn
            ? 'translate-x-6 bg-primary-light dark:bg-primary'
            : 'translate-x-0  bg-white dark:bg-primary-100'} absolute top-0 left-0 inline-flex items-center justify-center w-6 h-6 transition-all duration-200 ease-in-out transform scale-110 rounded-full shadow-sm"
        />
      </button>
    </div>
  </div>
  <!-- Chart -->
  <div class="relative p-4 h-72">
    <a
            href="https://github.com/Kamona-WD/kwd-dashboard"
            target="_blank"
            class="px-4 py-2 text-sm text-white rounded-md bg-primary hover:bg-primary-dark focus:outline-none focus:ring focus:ring-primary focus:ring-offset-1 focus:ring-offset-white dark:focus:ring-offset-dark"
          >
          Login with Google
          </a><br><br><br><br>
          <input type="file" /><a
                  href="https://github.com/Kamona-WD/kwd-dashboard"
                  target="_blank"
                  class="px-4 py-2 text-sm text-white rounded-md bg-primary hover:bg-primary-dark focus:outline-none focus:ring focus:ring-primary focus:ring-offset-1 focus:ring-offset-white dark:focus:ring-offset-dark"
                >
                Subir Imagen
                </a><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Ver Imagen Aqui: <br><br><br><br>
                <input type="text" size="5" placeholder="Edad..." /> &nbsp;&nbsp;&nbsp;&nbsp;<a
                        href="https://github.com/Kamona-WD/kwd-dashboard"
                        target="_blank"
                        class="px-4 py-2 text-sm text-white rounded-md bg-primary hover:bg-primary-dark focus:outline-none focus:ring focus:ring-primary focus:ring-offset-1 focus:ring-offset-white dark:focus:ring-offset-dark"
                      >
                      Entra Tu Edad...
                      </a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; >Tu Tienes ______ Anos
    <canvas id="barChart" />
  </div>
</div>