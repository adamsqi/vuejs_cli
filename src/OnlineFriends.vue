<template>
    <div id="online-friends">
        <h2>Online Friends</h2>
        <div v-for="(friend, index) in friends" :key="index">
            <span v-if="friend.online">{{ friend.name }}</span>
        </div>
    </div>
</template>

<script>
export default {
    name: 'OnlineFriends',
    data () {
        return {
            friends: [
                { name: 'Mario', online: true},
                { name: 'Adam', online: false},
                { name: 'Henry', online: true},
                { name: 'John', online: false}
            ]
        }
    }
}
</script>

<style>

</style>
