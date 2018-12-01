<template>
    <div class="col-xs-12 col-sm-6">
        <ul class="list-group">
            <app-server-status v-for="(server, index) in 5" :key="index" :index="index"></app-server-status>
        </ul>
    </div>
</template>

<script>
import ServerStatus from './ServerStatus.vue'
export default {
    components: {
        'app-server-status' : ServerStatus
    }
}
</script>