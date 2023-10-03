<template>
  <div class="grid">
    <div class="item div1"></div>
    <div class="item div2"></div>
    <div class="item div3"> Jip Erkelens</div>
    <div class="item div4">

    </div>
    <div class="item div5"></div>
    <div class="item div6"></div>
    <div class="item div7"></div>
  </div>
</template>

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
