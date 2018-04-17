
<template>
  <div class="container">
  	<h2>Blog Edit</h2>
  	<hr>

  	<div class="card">
  		<div class="card body">

        <div class="m-3">

          <form action="#">
            <div class="form-group">
              <label>Blog Title</label>
              <input type="text" class="form-control" placeholder="Title">
            </div>

            <div class="form-group">
            	<b-form-select v-model="selected" :options="options" class="mb-3" >
            		<template slot="first">
            			<option :value="null" disabled>-- Please select a project --</option>
            		</template>

            	</b-form-select>

            </div>

 
            <div class="form-group">
              <label>Blog Content</label>
              <textarea class="form-control"></textarea>
            </div>

            <div class="form-group">
              <label>Tags</label>
              <input class="form-control">
            </div>

            <button type="submit" class="btn btn-default">Save changes</button>
          </form> 

        </div>
  		</div>
  	</div>
  </div>
</template>

<!-- // // // //  -->

<script>
export default {
  name: 'layout',
  data () {
    return {
      selected: null,
      options: [
        { text: 'Observatory' },
        { text: 'Mergeable' },
        { text: 'Hedgehogs' }
      ]
    }
  }

}
</script>


