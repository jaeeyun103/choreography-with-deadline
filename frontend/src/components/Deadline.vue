<template>
    <div>
        <Date
            label="Deadline"
            v-model="value.deadline"
            :editMode="editMode"
        />
        <Number
            label="OrderId"
            v-model="value.orderId"
            :editMode="editMode"
        />
        <Date
            label="StartedTime"
            v-model="value.startedTime"
            :editMode="editMode"
        />
        <v-row class="ma-0 pa-0">
            <v-spacer></v-spacer>
            <v-btn width="64px" color="primary" @click="save">
                저장
            </v-btn>
        </v-row>
    </div>
</template>


<script>
import BaseEntity from './base-ui/BaseEntity.vue'

export default {
    name: 'Deadline',
    mixins:[BaseEntity],
    components:{
    },
    
    data: () => ({
        path: "deadlines",
        value: {
        }
    }),
    created(){
    },
    computed:{
    },
    methods: {
    },
}
</script>
