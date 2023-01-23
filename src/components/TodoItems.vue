<template>
    <div class="space-y-2">
        <TodoItem 
            v-for="todo in $store.state.todos" 
            v-bind:key="todo.id"
            v-bind:todo="todo"
        />
    </div>
</template>

<script>
import TodoItem from '@/components/TodoItem.vue';

export default {
    components: {TodoItem}
}
</script>