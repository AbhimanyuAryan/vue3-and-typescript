<template>
  <router-link :to="{ name: 'EventDetails', params: { id: event.id } }">
    <v-card class="mx-auto" max-width="344" outlined>
      <v-list-item three-line>
        <v-list-item-content>
          <div class="text-overline mb-4">
            @{{ event.time }} on {{ event.date }}
          </div>
          <v-list-item-subtitle>{{ event.title }}</v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>
    </v-card>
  </router-link>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  props: {
    event: {
      type: Object,
      required: true
    }
  }
})
</script>
