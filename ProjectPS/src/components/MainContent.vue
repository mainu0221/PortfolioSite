<template>
  <div class="md:ml-[25%] bg-white min-h-screen relative text-gray-700">
    <section class="h-screen flex flex-col justify-center items-center p-10 bg-gray-50">
      <h1 class="text-5xl font-bold mb-4 text-gray-900">
        코멘트 <span class="text-gray-400">or</span> 포부
      </h1>
      <p class="text-xl text-gray-500 mb-10">꾸준히 성장하는 개발자 000입니다.</p>

      <div class="flex gap-6">
        <button
          @click="moveTo('project-section')"
          class="px-8 py-4 bg-gray-800 text-white rounded-full font-bold text-lg hover:bg-emerald-600 transition shadow-lg transform hover:-translate-y-1"
        >
          Project
        </button>

        <button
          @click="moveTo('skill-section')"
          class="px-8 py-4 bg-white border-2 border-gray-300 text-gray-700 rounded-full font-bold text-lg hover:border-emerald-500 hover:text-emerald-500 transition shadow-lg transform hover:-translate-y-1"
        >
          Tech Stack
        </button>
      </div>
    </section>

    <section id="resume-section" class="py-24 px-8 md:px-20 border-t border-gray-100">
      <div
        class="flex flex-col md:flex-row md:items-end justify-between mb-16 border-b-4 border-emerald-100 pb-2"
      >
        <h2 class="text-3xl font-bold text-emerald-600">Resume</h2>

        <a
          href="/test.pdf"
          download="자기소개서서.pdf"
          class="mt-4 md:mt-0 flex items-center gap-2 px-5 py-2 bg-gray-800 text-white rounded-lg hover:bg-emerald-600 hover:-translate-y-1 transition shadow-md font-bold text-sm"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="2"
            stroke="currentColor"
            class="w-5 h-5"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M3 16.5v2.25A2.25 2.25 0 005.25 21h13.5A2.25 2.25 0 0021 18.75V16.5M16.5 12L12 16.5m0 0L7.5 12m4.5 4.5V3"
            />
          </svg>
          자기소개서서(PDF) 다운로드
        </a>
      </div>

      <div class="mb-16">
        <h3 class="text-xl font-bold text-gray-900 mb-6 flex items-center">
          <span class="w-2 h-8 bg-gray-800 mr-3 rounded-sm"></span>About Me
        </h3>
        <p class="text-lg leading-relaxed text-gray-600">
          안녕하세요. 사용자의 경험을 중요하게 생각하는 프론트엔드 개발자입니다.<br />
          새로운 기술을 배우는 것을 두려워하지 않으며, 동료와의 원활한 소통을 통해<br />
          함께 성장하는 개발 문화를 지향합니다.
        </p>
      </div>

      <div class="mb-16">
        <h3 class="text-xl font-bold text-gray-900 mb-6 flex items-center">
          <span class="w-2 h-8 bg-gray-800 mr-3 rounded-sm"></span>Education
        </h3>
        <ul class="space-y-8">
          <li>
            <div class="flex flex-col md:flex-row md:items-baseline md:justify-between mb-1">
              <h4 class="text-lg font-bold text-gray-800">안하공업전문대학교 (컴퓨터정보공학과)</h4>
              <span class="text-sm text-gray-500">2023.03 ~ 2026.02 (졸업예정)</span>
            </div>
            <p class="text-gray-600">학점: 4.1 / 4.5</p>
          </li>
          <li>
            <div class="flex flex-col md:flex-row md:items-baseline md:justify-between mb-1">
              <h4 class="text-lg font-bold text-gray-800">한서대학교 (항공전자공학)</h4>
              <span class="text-sm text-gray-500">2017.03 ~ 2022.08 (자퇴)</span>
            </div>
            <p class="text-gray-500 text-sm">
              - 전자 회로 및 임베디드 시스템 기초 학습 후, 소프트웨어 개발로 진로 변경
            </p>
          </li>
          <li>
            <div class="flex flex-col md:flex-row md:items-baseline md:justify-between mb-1">
              <h4 class="text-lg font-bold text-gray-800">계산공업고등학교 (컴퓨터정보전자과)</h4>
              <span class="text-sm text-gray-500">2014.03 ~ 2017.02 (졸업)</span>
            </div>
          </li>
        </ul>
      </div>

      <div>
        <h3 class="text-xl font-bold text-gray-900 mb-6 flex items-center">
          <span class="w-2 h-8 bg-gray-800 mr-3 rounded-sm"></span>Certificates
        </h3>
        <ul class="grid grid-cols-1 md:grid-cols-2 gap-4">
          <li class="bg-gray-50 p-4 rounded border border-gray-200">
            <strong class="block text-gray-900 mb-1">SQLD</strong>
            <span class="text-sm text-gray-500">한국데이터산업진흥원 | 2024.09</span>
          </li>
          <li class="bg-gray-50 p-4 rounded border border-gray-200">
            <strong class="block text-gray-900 mb-1">MOS Master</strong>
            <span class="text-sm text-gray-500">YBMIT | 2023.12</span>
          </li>
          <li class="bg-gray-50 p-4 rounded border border-gray-200">
            <strong class="block text-gray-900 mb-1">전자기능사</strong>
            <span class="text-sm text-gray-500">한국산업인력공단 | 2016.07</span>
          </li>
        </ul>
      </div>
    </section>

    <section id="project-section" class="py-24 px-8 md:px-20 bg-gray-50 border-t border-gray-200">
      <h2
        class="text-3xl font-bold mb-16 text-emerald-600 inline-block border-b-4 border-emerald-200 pb-2"
      >
        Projects
      </h2>

      <div class="space-y-12">
        <article
          class="bg-white p-8 rounded-xl shadow-sm hover:shadow-md transition cursor-pointer group"
          onclick="window.open('https://github.com')"
        >
          <div class="flex flex-col md:flex-row gap-8">
            <div
              class="w-full md:w-1/3 h-48 bg-gray-200 rounded-lg flex items-center justify-center text-gray-400 group-hover:bg-gray-300 transition"
            >
              이미지 미리보기
            </div>
            <div class="w-full md:w-2/3">
              <h3 class="text-2xl font-bold mb-3 group-hover:text-emerald-600 transition">
                나의 첫번째 프로젝트
              </h3>
              <p class="text-gray-600 mb-4 leading-relaxed">
                Vue.js와 Firebase를 활용하여 만든 실시간 채팅 서비스입니다. 사용자 경험을 위해 소켓
                통신을 최적화했습니다.
              </p>
              <div class="flex gap-2 flex-wrap">
                <span
                  class="px-3 py-1 bg-emerald-50 text-emerald-700 text-sm font-medium rounded-full"
                  >Vue.js</span
                >
                <span
                  class="px-3 py-1 bg-emerald-50 text-emerald-700 text-sm font-medium rounded-full"
                  >Firebase</span
                >
              </div>
            </div>
          </div>
        </article>

        <article
          class="bg-white p-8 rounded-xl shadow-sm hover:shadow-md transition cursor-pointer group"
          onclick="window.open('https://github.com')"
        >
          <div class="flex flex-col md:flex-row gap-8">
            <div
              class="w-full md:w-1/3 h-48 bg-gray-200 rounded-lg flex items-center justify-center text-gray-400 group-hover:bg-gray-300 transition"
            >
              이미지 미리보기
            </div>
            <div class="w-full md:w-2/3">
              <h3 class="text-2xl font-bold mb-3 group-hover:text-emerald-600 transition">
                쇼핑몰 웹사이트
              </h3>
              <p class="text-gray-600 mb-4 leading-relaxed">
                반응형 웹 디자인을 적용한 의류 쇼핑몰입니다. 결제 모듈 연동 경험이 있습니다.
              </p>
              <div class="flex gap-2 flex-wrap">
                <span
                  class="px-3 py-1 bg-emerald-50 text-emerald-700 text-sm font-medium rounded-full"
                  >React</span
                >
                <span
                  class="px-3 py-1 bg-emerald-50 text-emerald-700 text-sm font-medium rounded-full"
                  >Node.js</span
                >
              </div>
            </div>
          </div>
        </article>
      </div>
    </section>

    <section id="skill-section" class="py-24 px-8 md:px-20 border-t border-gray-200 bg-gray-50">
      <h2
        class="text-3xl font-bold mb-16 text-emerald-600 inline-block border-b-4 border-emerald-100 pb-2"
      >
        Tech Stack
      </h2>

      <div class="flex flex-wrap justify-center gap-6 text-center">
        <div
          class="w-40 p-6 bg-white border border-gray-200 rounded-xl hover:border-emerald-500 transition cursor-default group shadow-sm hover:shadow-md flex flex-col items-center"
        >
          <img
            src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg"
            alt="Python"
            class="w-16 h-16 mb-4 group-hover:scale-110 transition object-contain"
          />
          <div class="font-bold text-lg text-gray-700">Python</div>
        </div>

        <div
          class="w-40 p-6 bg-white border border-gray-200 rounded-xl hover:border-emerald-500 transition cursor-default group shadow-sm hover:shadow-md flex flex-col items-center"
        >
          <img
            src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/c/c-original.svg"
            alt="C"
            class="w-16 h-16 mb-4 group-hover:scale-110 transition object-contain"
          />
          <div class="font-bold text-lg text-gray-700">C</div>
        </div>

        <div
          class="w-40 p-6 bg-white border border-gray-200 rounded-xl hover:border-emerald-500 transition cursor-default group shadow-sm hover:shadow-md flex flex-col items-center"
        >
          <img
            src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/csharp/csharp-original.svg"
            alt="C#"
            class="w-16 h-16 mb-4 group-hover:scale-110 transition object-contain"
          />
          <div class="font-bold text-lg text-gray-700">C#</div>
        </div>

        <div
          class="w-40 p-6 bg-white border border-gray-200 rounded-xl hover:border-emerald-500 transition cursor-default group shadow-sm hover:shadow-md flex flex-col items-center"
        >
          <img
            src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg"
            alt="Java"
            class="w-16 h-16 mb-4 group-hover:scale-110 transition object-contain"
          />
          <div class="font-bold text-lg text-gray-700">Java</div>
        </div>

        <div
          class="w-40 p-6 bg-white border border-gray-200 rounded-xl hover:border-emerald-500 transition cursor-default group shadow-sm hover:shadow-md flex flex-col items-center"
        >
          <img
            src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg"
            alt="Git"
            class="w-16 h-16 mb-4 group-hover:scale-110 transition object-contain"
          />
          <div class="font-bold text-lg text-gray-700">Git/GitHub</div>
        </div>
      </div>
    </section>

    <div class="h-40"></div>
  </div>
</template>

<script setup>
const moveTo = (id) => {
  const el = document.getElementById(id)
  if (el) el.scrollIntoView({ behavior: 'smooth' })
}
</script>
