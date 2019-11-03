<template>
  <div>
    <treeselect
      :multiple="true"
      :flatten-search-results="true"
      :options="options"
      placeholder="Select 11 favourite(s)..."
      v-model="value"
      :defaultExpandLevel="Infinity"
      :defaultOpen="true"
      :openOnClick="true"
      openDirection="bottom"
      :z-index="3"
    />
    <treeselect
      :multiple="true"
      :flatten-search-results="true"
      :options="options"
      placeholder="Select 11 favourite(s)..."
      v-model="value"
      :defaultExpandLevel="Infinity"
      :defaultOpen="true"
      :openOnClick="true"
      openDirection="bottom"
      :z-index="2"
    />
    <pre class="result">{{ value }}</pre>
  </div>
</template>

<script>
export default {
  data: () => ({
    value: [],
    options: [
      {
        id: "fruits",
        label: "Fruits",
        children: [
          {
            id: "apple",
            label: "Adasdasfasdasdasdasdasdasdasaswdasdasqddaspple 🍎",
            isNew: true
          },
          {
            id: "grapes",
            label: "Grapes 🍇"
          },
          {
            id: "pear",
            label: "Pear 🍐"
          },
          {
            id: "strawberry",
            label: "Strawberry 🍓"
          },
          {
            id: "watermelon",
            label: "Watermelon 🍉"
          }
        ]
      },
      {
        id: "vegetables",
        label: "Vegetables",
        children: [
          // {
          //   id: 'corn',
          //   label: 'Corn 🌽'
          // },
          // {
          //   id: 'carrot',
          //   label: 'Carrot 🥕'
          // },
          // {
          //   id: 'eggplant',
          //   label: 'Eggplant 🍆'
          // },
          // {
          //   id: 'tomato',
          //   label: 'Tomato 🍅'
          // }
        ]
      }
    ]
  })
};
</script>
