<!DOCTYPE html>
<html lang="bn" class="bg-gray-100 dark:bg-gray-900">
<head>
  <meta charset="UTF-8" />
  <title>Shuvo All Tool</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <!-- Tailwind CSS CDN -->
  <script src="https://cdn.tailwindcss.com?version=3.4.1"></script>

  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+Bengali:wght@400;700&family=Roboto:wght@400;700&display=swap" rel="stylesheet">

  <!-- Initial Theme Load -->
  <script>
    const savedTheme = localStorage.getItem('theme') || 'light';
    document.documentElement.classList.toggle('dark', savedTheme === 'dark');
  </script>

  <style>
    body { opacity: 0; transition: opacity 0.5s ease-in-out; }
    body.loaded { opacity: 1; }
  </style>
</head>
<body class="font-['Noto Sans Bengali','Roboto',sans-serif] text-gray-800 dark:text-gray-100 transition-colors duration-300 ease-in-out">

  <!-- Loader -->
  <div id="loader" class="fixed inset-0 bg-white dark:bg-gray-900 flex items-center justify-center z-50">
    <div class="w-16 h-16 border-4 border-blue-500 border-t-transparent border-dashed rounded-full animate-spin"></div>
  </div>

  <!-- Header -->
  <header class="bg-blue-600 dark:bg-blue-800 text-white py-5 text-center text-3xl font-bold shadow-md">
    🌟 Shuvo All Tool 🌟
  </header>

  <!-- Notice -->
  <section id="notice" class="bg-yellow-100 dark:bg-yellow-300 text-yellow-900 max-w-3xl mx-auto mt-6 p-6 rounded-lg shadow-sm"></section>

  <!-- Theme Toggle Button -->
  <div class="text-center mt-4">
    <button id="toggleTheme"
      class="inline-flex items-center gap-2 bg-gray-200 dark:bg-gray-800 text-gray-800 dark:text-gray-100 px-4 py-2 rounded-full shadow hover:bg-gray-300 dark:hover:bg-gray-700 transition">
      🌗 থিম পরিবর্তন করুন
    </button>
  </div>

  <!-- Tools Grid -->
  <section id="tools" class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-5 gap-6 max-w-6xl mx-auto px-4 py-10 transition"></section>

  <!-- Footer -->
  <footer class="text-center text-sm text-gray-500 dark:text-gray-400 py-4">
    © 2025 Shuvo All Tool
  </footer>

  <!-- Firebase Script -->
  <script type="module">
    import { initializeApp } from "https://www.gstatic.com/firebasejs/9.23.0/firebase-app.js";
    import { getDatabase, ref, onValue } from "https://www.gstatic.com/firebasejs/9.23.0/firebase-database.js";

    const firebaseConfig = {
      apiKey: "AIzaSyDkqjA1Io411uidSZBLbYJlYHWGVY36zc8",
      authDomain: "shuvo-all-tools.firebaseapp.com",
      databaseURL: "https://shuvo-all-tools-default-rtdb.firebaseio.com/",
      projectId: "shuvo-all-tools",
      storageBucket: "shuvo-all-tools.appspot.com",
      messagingSenderId: "475600173705",
      appId: "1:475600173705:android:0251b1d46457dc4e806458"
    };

    const app = initializeApp(firebaseConfig);
    const db = getDatabase(app);

    // Load Notice
    const noticeRef = ref(db, 'Notice');
    onValue(noticeRef, (snapshot) => {
      const notice = snapshot.val();
      const noticeBox = document.getElementById('notice');
      if (notice) {
        noticeBox.innerHTML = `
          <h3 class="text-xl font-bold mb-2">${notice.title}</h3>
          <p class="text-base">${notice.body}</p>
        `;
      } else {
        noticeBox.innerHTML = "";
      }
    }, (error) => {
      console.error("Notice Load Error:", error);
    });

    // Load Tools
    const toolsRef = ref(db, 'Tools');
    onValue(toolsRef, (snapshot) => {
      const toolsDiv = document.getElementById('tools');
      toolsDiv.innerHTML = '';
      let hasTool = false;

      snapshot.forEach((child) => {
        const tool = child.val();
        if (tool.status === "active") {
          hasTool = true;
          toolsDiv.innerHTML += `
            <div role="button" tabindex="0" aria-label="${tool.name}" onclick="window.open('${tool.link}', '_blank')" 
              onkeypress="if(event.key==='Enter'){window.open('${tool.link}', '_blank')}" 
              class="bg-white dark:bg-gray-800 rounded-xl shadow hover:shadow-lg hover:-translate-y-1 transition transform cursor-pointer flex flex-col items-center p-4">
              <img loading="lazy" src="${tool.icon}" alt="${tool.name}" class="w-20 h-20 object-contain mb-3">
              <span class="text-center font-semibold text-gray-900 dark:text-gray-100">${tool.name}</span>
            </div>
          `;
        }
      });

      if (!hasTool) {
        toolsDiv.innerHTML = `<p class="col-span-full text-center text-gray-500 dark:text-gray-400">🔍 কোনো টুল পাওয়া যায়নি</p>`;
      }

      // Hide loader
      document.getElementById('loader').style.display = 'none';
      document.body.classList.add('loaded');
    }, (error) => {
      console.error("Tools Load Error:", error);
      document.getElementById('loader').style.display = 'none';
    });
  </script>

  <!-- Theme Toggle JS -->
  <script>
    document.addEventListener('DOMContentLoaded', () => {
      const themeToggle = document.getElementById('toggleTheme');

      themeToggle?.addEventListener('click', () => {
        const html = document.documentElement;
        const isDark = html.classList.contains('dark');

        html.classList.toggle('dark');
        localStorage.setItem('theme', isDark ? 'light' : 'dark');
      });

      // Fallback loader remove
      setTimeout(() => {
        document.getElementById('loader').style.display = 'none';
        document.body.classList.add('loaded');
      }, 800);
    });
  </script>

</body>
</html>
