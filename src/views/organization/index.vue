/* eslint-disable */ 
<template>
    <tree-table :data="data" :columns="columns" border/>    
</template>

<script>
export default {
    data() {
        return {
            data: [
                {
                    name: '1',
                    children: [
                        {
                            name: '1-1'
                        },
                        {
                            name: '1-2'
                        }
                    ]
                },
                {
                    name: '2'
                }
            ],
            columns: [
                {
                    label: 'Checkbox',
                    checkbox: true
                },
                {
                    label: '',
                    key: 'id',
                    expand: true
                },
                {
                    label: 'Event',
                    key: 'event',
                    width: 200,
                    align: 'left'
                },
                {
                    label: 'Scope',
                    key: 'scope'
                }
            ]
        }
    }
}
</script>

