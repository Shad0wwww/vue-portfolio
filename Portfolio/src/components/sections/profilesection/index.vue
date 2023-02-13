<template>
    <div class="container" style="padding: 2rem; justify-content: space-between;" id="profile">
        <div/>
        
        <div class="center">
            <ProfilePicture />
            <div class="profile">
            <h1 class="title">
                Magnus pins <span class="age">(16 y/o)</span>
            </h1>
            <h2 class="profession">
                
            </h2>
            </div>
         
        </div>
        
    </div>
</template>

<style scoped>
.center {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
.profile {
    margin-top: 1rem;
    text-align: center;
}
.title {
    font-size: 25px;
    font-weight: 700;
    color: var(--primary-color);
}
.title .age {
    font-size: 16px;
    font-weight: 500;
}
.profession {
    font-size: 16px;
    font-weight: 500;
    color: var(--secondary-color);
}
.socials {
    margin-top: 1rem;
    display: flex;
    flex-wrap: wrap;
    flex-direction: row;
    justify-content: center;
}
.scroll-arrow-box {
    display: flex;
    justify-content: center;
    align-items: center;   
}
.scroll-arrow {
    cursor: pointer;
    transition: transform 0.2s ease-in-out;
    color: var(--primary-color);
    border-radius: 9999px;
}
.scroll-arrow:hover {
    transform: scale(1.1);
    background-color: #FAF9F6;
}
</style>
<script lang="js">
    import ProfilePicture from './ProfilePicture.vue';
    
    export default ({
        name: "ProfileSection",
        components: {
            ProfilePicture
        } 
    })
</script>