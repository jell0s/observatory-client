<template>
  <div class="container">
    <PageHeader :title="model.name" />

    <div class="row">

      <div class="col-lg-3">
        <Sidebar :model="model"/>
      </div>

      <div class="col-lg-9">
        <Tech :model="model"/>
        <Bio :model="model"/>
        <Projects :model="model"/>
      </div>

    </div>

  </div>
</template>

<!-- // // // //  -->

<script>
import Sidebar from './sidebar'
import Tech from './tech'
import Bio from './bio'
import Projects from './projects'

export default {
  props: ['model'],
  components: { Sidebar, Tech, Bio, Projects }
}
</script>
