<template>
  <div class="flex flex-col w-screen h-full">
    <!-- Your name, profile picture and contact -->
    <HeadWrapper
      name="Khoo Bee Sze"
      title="Fresh Graduate"
      userImgURL="../img/resume_pic.JPG"
      phone="017 9788130"
      email="bckhoo0210@gmail.com"
    />
    <!-- About Me -->
    <AboutWrapper
      aboutMe="Hi, Thank you for the Live Seminar"
      linkedInURL="https://www.linkedin.com/in/khoobeesze/"
      languages="Campur"
      nationality="Malaysia"
      interest="Eat Sleep Play"
    />
    <!-- Working Experience -->
    <CareerWrapper>
      <template v-slot:career>
        <Career
          companyName="Precision Control Sdn Bhd"
          title="Trainee"
          startDate="June 2019"
          endDate="August 2019"
        >
          <!-- List of what you had did in the company -->
          <template v-slot:experience>
            <ul class="text-gray-600 list-inside list-disc mt-2 px-4">
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
            </ul>
          </template>
        </Career>

        <Career companyName="Pasar Kapar" title="Boss" startDate="15 years ago" endDate="Never">
          <!-- List of what you had did in the company -->
          <template v-slot:experience>
            <ul class="text-gray-600 list-inside list-disc mt-2 px-4">
              <li>Sleep</li>
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
            </ul>
          </template>
        </Career>

        <Career companyName="hi" title="Your Job Title" startDate="Start Date" endDate="End Date">
          <!-- List of what you had did in the company -->
          <template v-slot:experience>
            <ul class="text-gray-600 list-inside list-disc mt-2 px-4">
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
            </ul>
          </template>
        </Career>
      </template>
    </CareerWrapper>
    <!-- Achievement -->
    <AchievementWrapper project="2" client="haha" award="Sad"/>
    <!-- Portfolio -->
    <PortfolioWrapper>
      <template v-slot:portfolio>
        <div class="grid grid-cols-1 md:grid-cols-3">
          <ProjectCard
            imgUrl="../img/github.png"
            name="IDP "
            project="Smart Home Automation"
            projectURL="https://github.com"
          />

          <ProjectCard
            imgUrl="../img/github.png"
            name="Project Name"
            project="Project Type"
            projectURL="https://github.com"
          />

          <ProjectCard
            imgUrl="../img/github.png"
            name="Project Name"
            project="Project Type"
            projectURL="https://github.com"
          />
        </div>
      </template>
    </PortfolioWrapper>
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: "KHOO BEE SZE | Looking For Job HAHA"
    };
  }
};
</script>