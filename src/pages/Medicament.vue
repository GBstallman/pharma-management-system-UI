<template>
	<div class="parent">
		<div>
			<h1>Medicament</h1>
		</div>
		<div class="btn_panier">
			<button type="button" class="btn btn-primary btn-rounded">Ajouter</button>
		</div>
		<div class="table">
 <div>
    <table class="table table-striped table-responsive-md btn-table">

      <thead>
        <tr>
          <th>id</th>
          <th>Nom du produit</th>
          <th>Quantité</th>
          <th>Prix d'achat</th>
          <th>Lot</th>
          <th>Fournisseur</th>
          <th>Options</th>
        </tr>
      </thead>

      <tbody>
        <tr>
          <th scope="row">1</th>
          <td>Larry</td>
          <td>the Bird</td>
          <td>the Bird</td>
          <td>the Bird</td>
          <td>the Bird</td>
          <td>
            <button type="button" class="btn btn-outline-primary btn-sm m-0 waves-effect">Button</button>
          </td>
        </tr>
         <tr>
          <th scope="row">2</th>
          <td>Larry</td>
          <td>the Bird</td>
          <td>the Bird</td>
          <td>the Bird</td>
          <td>the Bird</td>
          <td>
            <button type="button" class="btn btn-outline-primary btn-sm m-0 waves-effect">Button</button>
          </td>
        </tr> 
        <tr>
          <th scope="row">3</th>
          <td>Larry</td>
          <td>the Bird</td>
          <td>the Bird</td>
          <td>the Bird</td>
          <td>the Bird</td>
          <td>
            <button type="button" class="btn btn-outline-primary btn-sm m-0 waves-effect">Button</button>
          </td>
        </tr>
      </tbody>

    </table>
  </div>
		</div>
	</div>
</template>
<script>

export default {
  name: 'Medicament',
  created() {

  },
  data() {
	return {
	}
  },
  props: {
   
  },
  methods: {
   
  },
};
	
</script>
<style scoped>
.table{
	margin-left: 2px;
	padding-left: 300px;
}
.btn_panier{
	margin-right: 100px;
	position: relative;
	float: right;
}
</style>