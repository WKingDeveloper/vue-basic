<template>
  <div>
    <div>
      <select name="" id="">
        <option :value="city.code" v-for="city in cities" :key="city.code">
          {{ city.title }}
        </option>
      </select>
    </div>

    <div>
      <table>
        <thead>
          <tr>
            <th>제품 번호</th>
            <th>제품명</th>
            <th>가격</th>
            <th>주문 수량</th>
            <th>합계</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="drink in drinkList" :key="drink.id">
            <td>{{ drink.id }}</td>
            <td>{{ drink.name }}</td>
            <td>{{ drink.price }}</td>
            <td><input type="number" v-model="drink.qty" /></td>
            <td>{{ drink.price * drink.qty }}</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      cities: [
        { title: '서울', code: '02' },
        { title: '부산', code: '051' },
        { title: '제주', code: '064' }
      ],
      drinkList: [
        {
          id: 1,
          name: '코카콜라',
          price: 700,
          qty: 1
        },
        {
          id: 2,
          name: '오렌지주스',
          price: 600,
          qty: 1
        },
        {
          id: 3,
          name: '사이다',
          price: 800,
          qty: 1
        },
        {
          id: 4,
          name: '밀키스',
          price: 500,
          qty: 1
        },
        {
          id: 5,
          name: '환타',
          price: 600,
          qty: 1
        }
      ]
    }
  },
  setup() {},
  created() {},
  mounted() {},
  unmounted() {},
  methods: {}
}
</script>
