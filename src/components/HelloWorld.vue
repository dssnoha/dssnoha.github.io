<script setup lang="ts">
import { ref } from 'vue'
import { Github, Mail, Computer } from 'lucide-vue-next'

const aboutMe = ref({
  name: 'Noha',
  description: "I'm Noha, an electroingenieur with a passion for technology and business. ",
  //link: 'https://nouricha.com',
  //linkText: 'Nouricha',
  //extra:
  //  "where I sell skincare products crafted with care. When I'm not building websites or creating products, you'll find me exploring new ideas and staying active.",
})

const projects = ref([
  'Nouricha - Skincare product line',
  'Vue.js 3 project with Vee-Validate form handling',
  'Energy ball mix for women packed with superfoods',
])

const skills = ref([
  'Software Development (Vue.js, c#, TypeScript)',
  'Business Management & E-commerce (Shopify)',
  'Marketing & Online Advertising',
])
function gottopage() {
  window.location.href = 'https://github.com/dssnoha'
}
function emailme() {
  window.location.href = 'mailto:dssnoha@gmail.com'
}
</script>

<template>
  <div class="min-h-screen bg-gradient-to-b from-purple-200 via-pink-100 to-white p-8">
    <header class="text-center mb-12">
      <h1 class="text-5xl font-extrabold text-purple-800 mb-4">Noha's World 🌸</h1>
      <p class="text-lg text-gray-600">Engineer | Dreamer</p>
    </header>

    <main class="grid grid-cols-1 md:grid-cols-2 gap-8 max-w-5xl mx-auto">
      <!-- About Me Card -->
      <div class="shadow-xl rounded-2xl p-6 bg-white">
        <h2 class="text-3xl font-bold text-purple-700 mb-2">About Me</h2>
        <p class="text-gray-700 text-base">
          {{ aboutMe.description }}
          <a :href="aboutMe.link" class="text-purple-500 underline" target="_blank">{{
            aboutMe.linkText
          }}</a
          >,
          {{ aboutMe.extra }}
        </p>
      </div>

      <!-- Projects Card -->
      <div class="shadow-xl rounded-2xl p-6 bg-white">
        <h2 class="text-3xl font-bold text-purple-700 mb-2">Projects</h2>
        <ul class="list-disc list-inside text-gray-700">
          <li v-for="(project, index) in projects" :key="index">{{ project }}</li>
        </ul>
      </div>

      <!-- Skills Card -->
      <div class="shadow-xl rounded-2xl p-6 bg-white">
        <h2 class="text-3xl font-bold text-purple-700 mb-2">💻 Tech Tech Skills:</h2>
        <ul class="list-disc list-inside text-gray-700">
          <div>
            <img
              src="https://camo.githubusercontent.com/25e4fea0521d29bddd8536b44c93ae3d30b25f36ed5139f2099fc7dc58bd6349/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f637373332d2532333135373242362e7376673f7374796c653d666c6174266c6f676f3d63737333266c6f676f436f6c6f723d7768697465"
              alt="CSS3"
              data-canonical-src="https://img.shields.io/badge/css3-%231572B6.svg?style=flat&amp;logo=css3&amp;logoColor=white"
              style="max-width: 100%"
            />
          </div>
          <div>
            <img
              src="https://camo.githubusercontent.com/13c01581ecdfac623e60b80b8f974efb37dadcdd28070f73d90968cfcf01fce3/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f747970657363726970742d2532333030374143432e7376673f7374796c653d666c6174266c6f676f3d74797065736372697074266c6f676f436f6c6f723d7768697465"
              alt="TypeScript"
              data-canonical-src="https://img.shields.io/badge/typescript-%23007ACC.svg?style=flat&amp;logo=typescript&amp;logoColor=white"
              style="max-width: 100%"
            />
          </div>
          <div>
            <img
              src="https://camo.githubusercontent.com/2ecce177af015ad041b013a2af08f434773f981a9c9a5b1fbb21b11fe45b3b2d/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f68746d6c352d2532334533344632362e7376673f7374796c653d666c6174266c6f676f3d68746d6c35266c6f676f436f6c6f723d7768697465"
              alt="HTML5"
              data-canonical-src="https://img.shields.io/badge/html5-%23E34F26.svg?style=flat&amp;logo=html5&amp;logoColor=white"
              style="max-width: 100%"
            />
          </div>
          <div>
            <img
              src="https://camo.githubusercontent.com/b481ebe6b89af68c74e4beabf39d44f389fa7fef5b160e5263edb7f5bd2559aa/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f632532332d2532333233393132302e7376673f7374796c653d666c6174266c6f676f3d637368617270266c6f676f436f6c6f723d7768697465"
              alt="C#"
              data-canonical-src="https://img.shields.io/badge/c%23-%23239120.svg?style=flat&amp;logo=csharp&amp;logoColor=white"
              style="max-width: 100%"
            />
          </div>
          <div>
            <img
              src="https://camo.githubusercontent.com/5c1d4693adb60b2b9c3e64e62865a31d280884c2d4e1333708fa20f074100c47/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f6a6176617363726970742d2532333332333333302e7376673f7374796c653d666c6174266c6f676f3d6a617661736372697074266c6f676f436f6c6f723d253233463744463145"
              alt="JavaScript"
              data-canonical-src="https://img.shields.io/badge/javascript-%23323330.svg?style=flat&amp;logo=javascript&amp;logoColor=%23F7DF1E"
              style="max-width: 100%"
            />
          </div>
          <div>
            <img
              src="https://camo.githubusercontent.com/aea764f3d25dd6d3a545789664f9cd1daf0f8c314eadaae0db4664b6780011c4/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f2e4e45542d3543324439313f7374796c653d666c6174266c6f676f3d2e6e6574266c6f676f436f6c6f723d7768697465"
              alt=".Net"
              data-canonical-src="https://img.shields.io/badge/.NET-5C2D91?style=flat&amp;logo=.net&amp;logoColor=white"
              style="max-width: 100%"
            />
          </div>
          <div>
            <img
              src="https://camo.githubusercontent.com/83fec3cfd4a3c732522dff68cf786e13e0dd63b9d1893478e088b736832d2dfa/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f6a6972612d2532333041304646462e7376673f7374796c653d666c6174266c6f676f3d6a697261266c6f676f436f6c6f723d7768697465"
              alt="Jira"
              data-canonical-src="https://img.shields.io/badge/jira-%230A0FFF.svg?style=flat&amp;logo=jira&amp;logoColor=white"
              style="max-width: 100%"
            />
          </div>
          <div>
            <img
              src="https://camo.githubusercontent.com/5345b371c895b151a12115bc4e4c2bfab5ae44a5310182ac28f7c4401be2eefb/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f506f73746d616e2d4646364333373f7374796c653d666c6174266c6f676f3d706f73746d616e266c6f676f436f6c6f723d7768697465"
              alt="Postman"
              data-canonical-src="https://img.shields.io/badge/Postman-FF6C37?style=flat&amp;logo=postman&amp;logoColor=white"
              style="max-width: 100%"
            />
          </div>
          <div>
            <img
              src="https://camo.githubusercontent.com/f448a0fea5f2a6f49b94996786808af11eeb15905cbf0cc49b3ecaebdaa267c7/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f2d537761676765722d253233436c6f6a7572653f7374796c653d666c6174266c6f676f3d73776167676572266c6f676f436f6c6f723d7768697465"
              alt="Swagger"
              data-canonical-src="https://img.shields.io/badge/-Swagger-%23Clojure?style=flat&amp;logo=swagger&amp;logoColor=white"
              style="max-width: 100%"
            />
          </div>
          <div>
            <img
              src="https://camo.githubusercontent.com/908a46646c0853eca8399a470b6e1d80b2e6b8404ce079ffb149ebba08180976/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f6769742d2532334630353033332e7376673f7374796c653d666c6174266c6f676f3d676974266c6f676f436f6c6f723d7768697465"
              alt="Git"
              data-canonical-src="https://img.shields.io/badge/git-%23F05033.svg?style=flat&amp;logo=git&amp;logoColor=white"
              style="max-width: 100%"
            />
          </div>
          <div>
            <img
              src="https://camo.githubusercontent.com/537a691f5001345a0bde6d7b601390b0604fbfa2369cab67787faca846f95d8f/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f6769746875622d2532333132313031312e7376673f7374796c653d666c6174266c6f676f3d676974687562266c6f676f436f6c6f723d7768697465"
              alt="GitHub"
              data-canonical-src="https://img.shields.io/badge/github-%23121011.svg?style=flat&amp;logo=github&amp;logoColor=white"
              style="max-width: 100%"
            />
          </div>
          <div>
            <img
              src="https://camo.githubusercontent.com/ece2c8006f454031406d976954fa050cf85392df8f87612884fade9a3d222593/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f6769746c61622d2532333138313731372e7376673f7374796c653d666c6174266c6f676f3d6769746c6162266c6f676f436f6c6f723d7768697465"
              alt="GitLab"
              data-canonical-src="https://img.shields.io/badge/gitlab-%23181717.svg?style=flat&amp;logo=gitlab&amp;logoColor=white"
              style="max-width: 100%"
            />
          </div>
          <div>
            <img
              src="https://camo.githubusercontent.com/c43f07e519458ff84e21c675bc59ce96f50b677addb0c410171343a17d16988c/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f61646f62652d2532334646303030302e7376673f7374796c653d666c6174266c6f676f3d61646f6265266c6f676f436f6c6f723d7768697465"
              alt="Adobe"
              data-canonical-src="https://img.shields.io/badge/adobe-%23FF0000.svg?style=flat&amp;logo=adobe&amp;logoColor=white"
              style="max-width: 100%"
            />
          </div>
          <div>
            <img
              src="https://camo.githubusercontent.com/68fdd20a91121eecd00b82a8bea1bd485907dd5b2512a02d515469333eb928d5/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f61646f626525323070686f746f73686f702d2532333331413846462e7376673f7374796c653d666c6174266c6f676f3d61646f626525323070686f746f73686f70266c6f676f436f6c6f723d7768697465"
              alt="Adobe Photoshop"
              data-canonical-src="https://img.shields.io/badge/adobe%20photoshop-%2331A8FF.svg?style=flat&amp;logo=adobe%20photoshop&amp;logoColor=white"
              style="max-width: 100%"
            />
          </div>
          <div>
            <img
              src="https://camo.githubusercontent.com/c1c5062b91943bdae4f0ee5412fc699bc1b11eb1da11458345c6e03225ccde10/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f43616e76612d2532333030433443432e7376673f7374796c653d666c6174266c6f676f3d43616e7661266c6f676f436f6c6f723d7768697465"
              alt="Canva"
              data-canonical-src="https://img.shields.io/badge/Canva-%2300C4CC.svg?style=flat&amp;logo=Canva&amp;logoColor=white"
              style="max-width: 100%"
            />
          </div>
          <div>
            <img
              src="https://camo.githubusercontent.com/0309026e387297fa47274f6b6f814148810c5c653678f4af7b14acd3a19fb640/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4d6172696144422d3030333534353f7374796c653d666c6174266c6f676f3d6d617269616462266c6f676f436f6c6f723d7768697465"
              alt="MariaDB"
              data-canonical-src="https://img.shields.io/badge/MariaDB-003545?style=flat&amp;logo=mariadb&amp;logoColor=white"
              style="max-width: 100%"
            />
          </div>
          <div>
            <img
              src="https://camo.githubusercontent.com/0e07b77861d08adcf9f80d43f0ae2d4ff1bc47989639ebde4f6fa61cdd3c1af0/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f6d7973716c2d3434373941312e7376673f7374796c653d666c6174266c6f676f3d6d7973716c266c6f676f436f6c6f723d7768697465"
              alt="MySQL"
              data-canonical-src="https://img.shields.io/badge/mysql-4479A1.svg?style=flat&amp;logo=mysql&amp;logoColor=white"
              style="max-width: 100%"
            />
          </div>
          <div>
            <img
              src="https://camo.githubusercontent.com/8730aa972ba3aafc4d0e4de21fe951706271e74d125bd8440ce62ef8071c7a9e/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f7675652e6a732d2532333335343935652e7376673f7374796c653d666c6174266c6f676f3d767565646f746a73266c6f676f436f6c6f723d253233344643303844"
              alt="Vue.js"
              data-canonical-src="https://img.shields.io/badge/vue.js-%2335495e.svg?style=flat&amp;logo=vuedotjs&amp;logoColor=%234FC08D"
              style="max-width: 100%"
            />
          </div>
          <div>
            <img
              src="https://camo.githubusercontent.com/65235d8f90a78848f1818fb24f93e316d246979e609b669a30f04a08b7c8a3df/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f626f6f7473747261702d2532333835313146412e7376673f7374796c653d666c6174266c6f676f3d626f6f747374726170266c6f676f436f6c6f723d7768697465"
              alt="Bootstrap"
              data-canonical-src="https://img.shields.io/badge/bootstrap-%238511FA.svg?style=flat&amp;logo=bootstrap&amp;logoColor=white"
              style="max-width: 100%"
            />
          </div>

          <!-- <li v-for="(skill, index) in skills" :key="index">{{ skill }}</li> -->
        </ul>
      </div>

      <!-- Contact Card -->
      <div class="shadow-xl rounded-2xl p-6 bg-white">
        <h2 class="text-3xl font-bold text-purple-700 mb-4">Get in Touch</h2>
        <div class="flex space-x-4">
          <button
            @click="emailme()"
            class="border border-gray-300 rounded-lg px-4 py-2 flex items-center space-x-2"
          >
            <Mail class="w-5 h-5" />
            <span>Email Me</span>
          </button>
          <button
            @click="gottopage()"
            class="border border-gray-300 rounded-lg px-4 py-2 flex items-center space-x-2"
          >
            <Github class="w-5 h-5" />
            <span>GitHub</span>
          </button>
        </div>
      </div>
    </main>

    <footer class="text-center mt-12 text-gray-500">
      <p>&copy; 2025 Noha. All rights reserved.</p>
    </footer>
  </div>
</template>
