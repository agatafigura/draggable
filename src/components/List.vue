<template>
  <div class="row">
    <div class="col-3" id="list1">
      <h3>Tasks</h3>
      <draggable
        class="list-group list1"
        :list="list1"
        :group="{ name: 'tasks', pull: 'clone', put: false }"
        @change="log"
      >
        <div
          class="list-group-item"
          v-for="element in list1"
          :key="element.name"
        >

          {{ element.name }}
        </div>
        
      </draggable>
    </div>

    <div class="col-3" id="list2">
      <h3>To do</h3>
      <draggable
        class="list-group list2"
        :list="list2"
        group="tasks"
        @change="log"
      >
        <div
          class="list-group-item"
          v-for="element in list2"
          :key="element.name"
        >
          {{ element.name }}
        </div>
      </draggable>
    </div>

    <div class="col-3" id="list3">
      <h3>Doing</h3>
      <draggable
        class="list-group list3"
        :list="list3"
        group="tasks"
        @change="log"
      >
        <div
          class="list-group-item"
          v-for="element in list3"
          :key="element.name"
        >
        
          {{ element.name }}
        </div>
      </draggable>
    </div>
   

    <div class="col-3" id="list4">
      <h3>Done</h3>
      <draggable
        class="list-group list4"
        :list="list4"
        group="tasks"
        @change="log"
      >
        <div
          class="list-group-item"
          v-for="element in list4"
          :key="element.name"
        >
          {{ element.name }}
        </div>
      </draggable>
    </div>

    <!-- <rawDisplayer class="col-3" :value="list1" title="List 1" />

    <rawDisplayer class="col-3" :value="list2" title="List 2" /> -->
  </div>
</template>
<script>
import draggable from "vuedraggable";
export default {
  name: "clone",
  display: "Clone",
  order: 2,
  components: {
    draggable,
  },

  data() {
    return {
      list1: [
        { name: "Wash dishes", id: 1 },
        { name: "Clean the kitchen", id: 2 },
        { name: "Send an email", id: 3 },
        { name: "Mop the floors", id: 4 },
         { name: "Walk the dog", id: 5 },
        { name: "Water the plants", id: 6 },
        { name: "Make dinner", id: 7 },
      ],
      list2: [],
      list3: [],
      list4: [],
    };
  },
  methods: {
    log: function (evt) {
      window.console.log(evt);
    },
  },
};
</script>
