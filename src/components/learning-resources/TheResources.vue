<template>
    <base-card>
      <base-button @click="setSelectedTab('stored-resources')">Stored Resources</base-button>
      <base-button @click="setSelectedTab('add-resources')">Add Resources</base-button> 
    </base-card>
    <component :is="selectedTab"></component>
</template>

<script>
import StoredResources from './StoredResources';
import AddResources from './AddResources';

export default {
    components: {
        StoredResources,
        AddResources
    },
    data() {
        return {
            selectedTab: 'stored-resources',
            storedResources: [
            {
                id: 'official-guide',
                title: 'Official Guide',
                description: 'The official Vue.js documentation.',
                link: 'https://vuejs.org',
            },
            {
                id: 'google',
                title: 'Google',
                description: 'Learn to google...',
                link: 'https://google.org',
            },
        ],
        }
    },
    provide() {
        return {
            resources: this.storedResources
        }
    },
    methods: {
        setSelectedTab(tab) {
            this.selectedTab = tab;
        }
    }
}
</script>

<style scoped>

</style>