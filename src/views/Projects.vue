<template>
  <div class="projects">
    <h1 class="subheading grey--text">Projects</h1>

    <v-container fluid class="my-5">
      <v-expansion-panel>
        <v-expansion-panel-content v-for="project in projects" :key="project.title">
          <template v-slot:header>
            <div>{{project.title}}</div>
          </template>
          <v-card>
            <v-card-text class="px-4 grey--text">
              <div class="font-weight-bold">due by {{project.due}}</div>
              <div>{{project.content}}</div>
            </v-card-text>
          </v-card>
        </v-expansion-panel-content>
      </v-expansion-panel>
    </v-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      projects: [
        {
          title: "Design a new website",
          person: "AqingCyan",
          due: "11th April 2019",
          status: "onging",
          content:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Animi, consectetur! Quam nostrum laborum perferendis sequi adipisci, laudantium dicta dolor beatae neque molestiae eligendi ad commodi nulla alias similique libero maiores."
        },
        {
          title: "Code up the homepage",
          person: "Xuekaiqi",
          due: "11th April 2019",
          status: "complete",
          content:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Animi, consectetur! Quam nostrum laborum perferendis sequi adipisci, laudantium dicta dolor beatae neque molestiae eligendi ad commodi nulla alias similique libero maiores."
        },
        {
          title: "Design video thumbnails",
          person: "Cyan",
          due: "11th April 2019",
          status: "onging",
          content:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Animi, consectetur! Quam nostrum laborum perferendis sequi adipisci, laudantium dicta dolor beatae neque molestiae eligendi ad commodi nulla alias similique libero maiores."
        },
        {
          title: "Wait a hr call",
          person: "CyanAqing",
          due: "10th April 2019",
          status: "overdue",
          content:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Animi, consectetur! Quam nostrum laborum perferendis sequi adipisci, laudantium dicta dolor beatae neque molestiae eligendi ad commodi nulla alias similique libero maiores."
        }
      ]
    };
  },
  computed: {
    myProjects() {
      return this.projects.filter(project => {
        return project.person === 'AqingCyan'
      })
    }
  },
};
</script>

<style scoped>
</style>
