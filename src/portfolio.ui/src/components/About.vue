<template>
  <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Role</template>

    <div class="about-sub-title">Software Developer</div>
    Currently I work for a digital transformation consultancy. In this time I
    have worked on a no code sass product, an ERP platform for a utilities
    provider and most recently teaching this years Academy intake technologies
    and concepts such as TypeScript, C#, TDD and Agile/ SCRUM.
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <ToolingIcon />
    </template>
    <template #heading>Skills</template>

    My main skillset comprises of C#, TypeScript, SQL, Vue.js, ASP.NET Core,
    Azure DevOps and Agile/ SCRUM methodologies.
    <div class="skills-exam">
      I've completed some Microsoft exams to test my skills which were really
      fun!
      <ul class="exam-list">
        <li>
          AZ204<img
            class="exam-certificate"
            src="@/assets/az204.jpg"
            alt="AZ400 certificate"
          />
        </li>
        <li>
          AZ400
          <img
            class="exam-certificate"
            src="@/assets/az400.jpg"
            alt="AZ400 certificate"
          />
        </li>
      </ul>
    </div>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <EcosystemIcon />
    </template>
    <template #heading>New Technologies</template>

    I always like the challenge of learning something new, some of the
    technologies and languages that I am currently looking into in my spare time
    are Blockchains, Microservices and GoLang.
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <CommunityIcon />
    </template>
    <template #heading>Interests</template>

    Outside of work I love keeping busy. Whether it's going to the gym and
    working out in my lunch, playing golf on an evening or anything related to
    food whether that's eating out somewhere new or making something delicious
    at home, especially my favourite - homemade pizza 🤤
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <LinkIcon />
    </template>
    <template #heading>Links</template>
    Check out my
    <a target="_blank" :href="gitHubUrl">GitHub</a> and
    <a target="_blank" :href="linkedinUrl">Linkedin</a> for more!
  </WelcomeItem>
</template>

<script setup lang="ts">
import WelcomeItem from "./WelcomeItem.vue";
import DocumentationIcon from "./icons/IconDocumentation.vue";
import ToolingIcon from "./icons/IconTooling.vue";
import EcosystemIcon from "./icons/IconEcosystem.vue";
import CommunityIcon from "./icons/IconCommunity.vue";
import LinkIcon from "./icons/IconLink.vue";
import SupportIcon from "./icons/IconSupport.vue";

const gitHubUrl: string = import.meta.env.VITE_GITHUB_URL;
const linkedinUrl: string = import.meta.env.VITE_LINKEDIN_URL;
</script>

<style lang="scss" scoped>
.about-sub-title {
  padding-bottom: 5px;
  font-size: 1.1rem;
  font-style: oblique;
}

.skills-exam {
  padding: 10px 0;
  .exam-list {
    list-style-type: none;
    .exam-certificate {
      height: 64px;
      width: 64px;
    }
  }
}

.other-links {
  list-style-type: disc;
}
</style>
