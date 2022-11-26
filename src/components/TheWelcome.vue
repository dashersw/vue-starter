<script>
import WelcomeItem from "./WelcomeItem.vue";
import DocumentationIcon from "./icons/IconDocumentation.vue";
import ToolingIcon from "./icons/IconTooling.vue";
import EcosystemIcon from "./icons/IconEcosystem.vue";
import CommunityIcon from "./icons/IconCommunity.vue";
import SupportIcon from "./icons/IconSupport.vue";

export default {
  components: {
    WelcomeItem,
    DocumentationIcon,
    ToolingIcon,
    EcosystemIcon,
    CommunityIcon,
    SupportIcon,
  },
};
</script>

<template lang="pug">
welcome-item
  template(#icon='')
    documentation-icon
  template(#heading='') Documentation
  | Vue’s&nbsp;
  a(href='https://vuejs.org/' target='_blank' rel='noopener') official documentation
  |  provides you with all information you need to get started.
welcome-item
  template(#icon='')
    tooling-icon
  template(#heading='') Tooling
  | This project is served and bundled with&nbsp;
  a(href='https://vitejs.dev/guide/features.html' target='_blank' rel='noopener') Vite
  | . The recommended IDE setup is&nbsp;
  a(href='https://code.visualstudio.com/' target='_blank' rel='noopener') VSCode
  |  +&nbsp;
  a(href='https://github.com/johnsoncodehk/volar' target='_blank' rel='noopener') Volar
  | . If you need to test your components and web pages, check out&nbsp;
  a(href='https://www.cypress.io/' target='_blank' rel='noopener') Cypress
  |  and&nbsp;
  a(href='https://on.cypress.io/component' target='_blank') Cypress Component Testing
  | .
  br
  | More instructions are available in&nbsp;
  code README.md
  | .
welcome-item
  template(#icon='')
    ecosystem-icon
  template(#heading='') Ecosystem
  | Get official tools and libraries for your project:&nbsp;
  a(href='https://pinia.vuejs.org/' target='_blank' rel='noopener') Pinia
  | ,&nbsp;
  a(href='https://router.vuejs.org/' target='_blank' rel='noopener') Vue Router
  | ,&nbsp;
  a(href='https://test-utils.vuejs.org/' target='_blank' rel='noopener') Vue Test Utils
  | , and&nbsp;
  a(href='https://github.com/vuejs/devtools' target='_blank' rel='noopener') Vue Dev Tools
  | . If you need more resources, we suggest paying&nbsp;
  a(href='https://github.com/vuejs/awesome-vue' target='_blank' rel='noopener') Awesome Vue
  |  a visit.
welcome-item
  template(#icon='')
    community-icon
  template(#heading='') Community
  | Got stuck? Ask your question on&nbsp;
  a(href='https://chat.vuejs.org' target='_blank' rel='noopener') Vue Land
  | , our official Discord server, or&nbsp;
  a(href='https://stackoverflow.com/questions/tagged/vue.js' target='_blank' rel='noopener') StackOverflow
  | . You should also subscribe to&nbsp;
  a(href='https://news.vuejs.org' target='_blank' rel='noopener') our mailing list&nbsp;
  | and follow the official&nbsp;
  a(href='https://twitter.com/vuejs' target='_blank' rel='noopener') @vuejs&nbsp;
  | twitter account for latest news in the Vue world.
welcome-item
  template(#icon='')
    support-icon
  template(#heading='') Support Vue
  | As an independent project, Vue relies on community backing for its
  | sustainability. You can help us by&nbsp;
  a(href='https://vuejs.org/sponsor/' target='_blank' rel='noopener') becoming a sponsor
  | .
</template>
