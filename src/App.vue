<template>
    <div id="app" class="container">
        <profile-card :name="profile1.name" :pic-url="profile1.picUrl" :alt-text="profile1.altText"></profile-card>
        <profile-card :name="profile2.name" :pic-url="profile2.picUrl" :alt-text="profile2.altText"></profile-card>
        <profile-card :name="profile3.name" :pic-url="profile3.picUrl" :alt-text="profile3.altText"></profile-card>
    </div>
</template>

<script>
import ProfileCard from "@/components/profileCard";

export default {
    name: 'App',
    components: { ProfileCard },
    data: function() {
        return {
            profile1: {
                name: "Susan Cox",
                picUrl: "assets/portrait1.jpg",
                altText: "Susan Cox's profile"
            },
            profile2: {
                name: "John Calcote",
                picUrl: "assets/portrait2.jpg",
                altText: "John Calcote's profile"
            },
            profile3: {
                name: "Charlotte Clinton",
                picUrl: "assets/portrait3.jpg",
                altText: "Charlotte Clinton's profile"
            },
        };
    }
}
</script>
