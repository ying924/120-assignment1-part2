<template>
  <div id="detail">

        <table cellspacing="5" cellpadding="5">
          <template  v-for="p in products" :key="p.name">
            <tr>
                <th >
                    <span><img class="resultImage" :src="p.img" /></span>
                </th>
                <th>
                    <span>{{p.name}}</span>
                </th>
                <th>
                    <span> $ {{p.price}}</span>
                </th>
            </tr>
            </template>
        </table>
    </div>
</template>

<script>
export default {
  name: "productListItems",
  props: ['products']
}
</script>

<style>
.resultImage {
    border-radius: 8px;
    border: 1px solid #ddd;
    padding: 5px;
    max-width: 30%;
}
</style>