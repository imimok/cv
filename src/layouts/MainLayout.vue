<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar>
    <!--     <q-btn
          flat
          dense
          round
          icon="menu"
          aria-label="Menu"
          @click="leftDrawerOpen = !leftDrawerOpen"
        />
 -->
          <q-toolbar-title>
            Welcome to My CV
          </q-toolbar-title>
            <div>Quasar v{{ $q.version }}</div>
      </q-toolbar>
<!--
          <q-toolbar>
            <q-breadcrumbs active-color="white" style="font-size: 16px">
              <q-breadcrumbs-el label="Home" icon="home" />
          </q-breadcrumbs>
        </q-toolbar> -->
    </q-header>
<!--     <q-drawer
      v-model="leftDrawerOpen"
      show-if-above
      bordered
      content-class="bg-grey-1"
    >
      <q-list>
        <q-item-label
          header
          class="text-grey-8"
        >
          Essential Links
        </q-item-label>
        <EssentialLink
          v-for="link in essentialLinks"
          :key="link.title"
          v-bind="link"
        />
      </q-list>
    </q-drawer> -->

 <!--    <q-page-container>
              <q-page padding>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugit nihil praesentium molestias a adipisci, dolore vitae odit, quidem consequatur optio voluptates asperiores pariatur eos numquam rerum delectus commodi perferendis voluptate?
          </p>
          place QPageScroller at end of page
          <q-page-scroller position="bottom-right" :scroll-offset="100" :offset="[10, 10]">
            <q-btn fab icon="keyboard_arrow_up" color="accent" />
          </q-page-scroller>
        </q-page>
    </q-page-container> -->
<q-page-container>

    <div class="q-px-lg q-pb-md">
    <q-timeline :layout="layout" :side="side" color="secondary">
      <q-timeline-entry heading>
        Education History
      </q-timeline-entry>

      <q-timeline-entry
        title="Exchange Student Programme"
        subtitle="September 2014 - January 2015"
        side="left"
        icon="las la-university"
      >
        <div>
          Bachelor's degree
          Computer Software Engineering
          Year: 2014- 2015
          Grade: 3.20
          Activities: University of Sriwijaya Exchange Program 2014
        </div>
      </q-timeline-entry>

      <q-timeline-entry
        title="Graduated from University of Sriwijaya"
        subtitle="December 08th, 2016"
        side="left"
        icon="las la-university"
      >
        <div>
          Bachelor's degree
          Computer and Information Systems Security/Information
          Year: 2011 - 2016
          Grade: 3.30
        </div>
      </q-timeline-entry>

      <q-timeline-entry heading>
        Work Experience
      </q-timeline-entry>

      <q-timeline-entry
        title="PT. Cira International"
        subtitle="May 2017 - January 2018"
        side="right"
        icon="las la-briefcase"
        color="positive"
      >
        <div>
          Tittle: Project Administrator
          Description: responsible to handle documents of project and recap all transactions of the project
        </div>
      </q-timeline-entry>

      <q-timeline-entry
        title="PT. Bumi Amartha Teknologi Mandiri"
        subtitle="February 2019 - March 2019"
        side="right"
        icon="las la-school"
        color="positive"
      >
        <div>
          Tittle: Training Java and SQL
          Description: In the first month learning Java and SQL and in the second month learn about how to involve in a project, handle project, manage the team
        </div>
      </q-timeline-entry>

      <q-timeline-entry
        title="PT. Bumi Amartha Teknologi Mandiri"
        subtitle="April 2019 - Now"
        side="right"
        icon="las la-briefcase"
        color="positive"
      >
        <div>
          Tittle: Junior Business Analyst
          Description: Part of Research and Development Team, help Project Manager to design Functional Specification Design, Database, Business Process of the product. Focus to Quality Assurance and Business Process of the product
        </div>
      </q-timeline-entry>

    </q-timeline>
  </div>
</q-page-container>

  </q-layout>
</template>

<script lang="ts">
// import EssentialLink from 'components/EssentialLink.vue'

// const linksData = [
//   {
//     title: 'LinkedIn',
//     caption: 'linkedin.com',
//     icon: 'ion-logo-linkedin',
//     link: 'https://www.linkedin.com/in/trismi-indah-nuraini-74477b12a/'
//   },
//   {
//     title: 'Instagram',
//     caption: 'instagram.com',
//     icon: 'ion-logo-instagram',
//     link: 'https://www.instagram.com/imimok/'
//   },
//   {
//     title: 'Discord',
//     caption: 'username:momomokkk#3842',
//     icon: 'lab la-discord'
//   },
//   {
//     title: 'Facebook',
//     caption: 'facebook.com',
//     icon: 'ion-logo-facebook',
//     link: 'https://www.facebook.com/trismi.i.nuraini'
//   },
//   {
//     title: 'Twitter',
//     caption: 'twitter.com',
//     icon: 'ion-logo-twitter',
//     link: 'https://twitter.com/imoookk'
//   }
// ]

// import { defineComponent, ref } from '@vue/composition-api'

// export default defineComponent({
//   name: 'MainLayout',
//   components: { EssentialLink },
//   setup () {
//     const leftDrawerOpen = ref(false)
//     const essentialLinks = ref(linksData)

//     return { leftDrawerOpen, essentialLinks }
//   }
// })

export default {
  data () {
    return {
      layout: 'loose',
      side: ''
    }
  }
}
</script>
