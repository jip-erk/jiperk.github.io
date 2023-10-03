<template>
    <div class="grid">
        <div class="item div1">
            <Icon name="mdi:github" />
            github
        </div>
        <div class="item div2">
            <Icon name="mdi:spotify" />
            spotify
        </div>
        <div class="item div3"> Jip Erkelens</div>
        <div class="item div4">
            <Icon name="material-symbols:mail" />
            email
        </div>
        <div class="item div5">
            <Icon name="mdi:linkedin" />
            linkedin
        </div>
        <div class="item div6">
            <Icon name="mdi:twitter" />
            twitter
        </div>
        <div class="item div7">
            <Icon name="mdi:instagram" />
            instagram
        </div>
    </div>

    <Teleport to="body">
        <div class="cookie" v-if="cookie">
            <Icon size="75px" name="material-symbols:cookie" />
            <div class="cookie-content">
                <p>This website uses cookies to ensure you get the best experience on our website. By continuing to use
                    this
                    website, you consent to our use of these cookies. For more information on cookies, please read our
                    <a href="/privacy-policy">Privacy Policy</a>.
                </p>
                <button @click="cookie = false">Accept</button>
            </div>
        </div>
    </Teleport>
</template>
  
<script lang="ts" setup>
const cookie = ref(true)
</script>
  
<style>
.grid {
    height: 100vh;
    width: 100%;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(3, 1fr);
    grid-column-gap: 0px;
    grid-row-gap: 0px;
}

.item {
    background-color: #101010;
    border-radius: .75rem;
    border: 1px solid #242424;
    margin: 1rem;
    font-size: 30px;
    text-align: center;
    color: aliceblue;
    font-size: 2.5rem;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 1rem;

}

.cookie {
    gap: 4rem;
    display: flex;
    align-items: center;
    padding: 0 4rem;
    height: 150px;
    background-color: black;
    border-radius: .25rem;
    border: 1px solid #242424;
    color: white;
    margin: 4rem;
    position: absolute;
    right: 0;
    bottom: 0;
}

a {
    color: #4e8ff7;
}

button {
    outline: none;
    border: none;
    background-color: #4e8ff7;
    padding: .5rem 1rem;
    border-radius: .15rem;
}

.div1 {
    grid-area: 1 / 1 / 2 / 3;
}

.div2 {
    grid-area: 2 / 1 / 3 / 2;
}

.div3 {
    grid-area: 2 / 2 / 3 / 3;
}

.div4 {
    grid-area: 1 / 3 / 2 / 4;
}

.div5 {
    grid-area: 3 / 2 / 4 / 4;
}

.div6 {
    grid-area: 3 / 1 / 4 / 2;
}

.div7 {
    grid-area: 2 / 3 / 3 / 4;
}
</style>
  