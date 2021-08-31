<template>
  <div>
    <div id="search">  
        <div>
            <input type="text" required="required" placeholder="name" name="keyword" />
            <button type="button">search</button>
            <button>asc</button>
            <button>desc</button>
        </div>
        <div>
            <ul>
                <li>
                    <span>area</span>
                    <select>
                        <option value="Sydney">Sydney</option>
                        <option value="Brisbane">Brisbane</option>
                        <option value="Melbourne">Melbourne</option>
                    </select>
                </li>
                <li>
                    <span>price range</span>
                    <input id="price_start" type="number"/>-
                    <input id="price_end" type="number">
                </li>
                <li>
                    <span>date range</span>
                    <input type="date" id="date_star"/>-
                    <input type="date" id="date_end"/>
                </li>
            </ul>
        </div>
    </div>
    <ProductListItem :products=products></ProductListItem>
    <div class="page">
        <a href="" title="pre">pre</a>
        <a class="num cur" href="" title="1">1</a>
        <a class="num" href="" title="2">2</a>
        <a class="num" href="" title="3">3</a>
        <a class="num" href="" title="4">4</a>
        <a class="num" href="" title="5">5</a>
        <a href="" title="next">next</a>
    </div>
  </div>
</template>

<script>
import ProductListItem from '@/components/ProductListItem.vue';
export default {
  name: 'productListItem',
  components: {
    ProductListItem,
  },
  data() {
    return {
      products: [
        {name: 'macbook air', price: 1350, img: 'https://m.media-amazon.com/images/I/71CGF458KbL._AC_UL320_.jpg'},
        {name: 'macbook air', price: 1550, img: 'https://m.media-amazon.com/images/I/71CGF458KbL._AC_UL320_.jpg'},
        {name: 'macbook air', price: 1258, img: 'https://m.media-amazon.com/images/I/71CGF458KbL._AC_UL320_.jpg'},
      ]
    }
  }
}
</script>

<style>
li {
  list-style: none;
}

.page {
    width: 928px; 
    display: table; 
    padding: 15px 0px 8px; 
    text-align: center; 
    font-size: 12px;
    margin: 0 auto;
}
.page a {
  width: auto; 
  height: 19px; 
  line-height: 19px; 
  padding: 0px 10px;
  margin: 0px 5px; 
  display: inline-block; 
  color: #7f7f7f; 
  background-color: #fff; 
  border: 1px solid #7f7f7f;
  }

.page a.num {
    font-family: Arial; 
    padding: 0px 6px;
}

.page a:hover, .page a.cur {
    background-color: #9c0004; 
    color: #fff; 
    border: 1px solid #9c0004;
}
</style>