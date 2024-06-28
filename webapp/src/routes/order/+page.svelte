<script>
	import {Grid, Button, TextInput, NativeSelect} from '@svelteuidev/core'
</script>

<div>
   <h2>Make an order</h2>
   <p>You can order a furniture here. If we have enough the delivery is instant, for the rest you'll need to wait until it's produced.</p>
   <div class="form">
      <Grid>
         <Grid.Col span={12}>
            <TextInput label="Your name" description="Input your name" />
         </Grid.Col>
         <Grid.Col span={12}>
            <NativeSelect data={['Svelte', 'React', 'Vue', 'Angular', 'Solid']} 
               placeholder="Pick one"
               label="Product"
               description="Select product to order"
            />
         </Grid.Col>
         <Grid.Col span={12}>
            <TextInput label="Amount" description="Choose amount to order" />
         </Grid.Col>
         <Grid.Col span={12} >
            <Button>Make order</Button>
         </Grid.Col>
      </Grid>
   </div>
</div>

<style>
   .form {
      width: 30%;
   }
</style>