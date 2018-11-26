<template>
    <div id="all-friends">
        <h2>All Friends</h2>
        <div v-for="(friend, index) in friends" :key="index">
            <span>{{ friend.name }}</span>
        </div>
    </div>
</template>

<script>
export default {
    name: 'AllFriends',
    data () {
        return {
            friends: [
                { name: 'Mario', online: true},
                { name: 'Adam', online: true},
                { name: 'Henry', online: true},
                { name: 'John', online: true}
            ]

        }
    }
}
</script>

<style>

</style>
