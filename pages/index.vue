<template>
  <div>
    <p class="line-1 anim-typewriter">Not yet ready !!!!</p>
    <div
      class="wrapper"
    >Lorem ipsum dolor sit, amet consectetur adipisicing elit. Perferendis libero voluptates quam dolores illo laudantium vel, veritatis illum officia exercitationem harum sequi tenetur iusto minus voluptate numquam corrupti voluptatibus fuga. Fugiat deserunt laborum, molestiae rerum incidunt atque. Animi aspernatur, inventore error autem atque assumenda exercitationem, nihil laborum quibusdam optio voluptates fugit deserunt debitis labore repudiandae ad necessitatibus fuga dicta, eos quae rem? Repellendus temporibus atque magni. Nostrum omnis consequuntur iusto qui error odio ducimus, ad reiciendis, deleniti sunt fugiat aliquam suscipit quam debitis tempora quae adipisci quas numquam possimus? At, impedit dolore ex officia ab cupiditate facilis? Aliquam cum, explicabo consequuntur recusandae veniam minima aliquid doloremque voluptas quidem possimus facere voluptatem officiis qui ullam unde illum nemo ea quibusdam molestiae accusantium repellat tenetur, non corporis! Debitis voluptate eius alias animi expedita atque porro odit tempora voluptatum accusamus! Sapiente, explicabo labore quaerat sit, eum quae, incidunt similique quas laboriosam soluta tenetur impedit obcaecati natus repudiandae ab ratione modi possimus odit alias quos! Praesentium debitis distinctio libero tenetur iusto perferendis impedit neque. Officiis recusandae ab magni, aliquam cumque labore dolorem harum deserunt numquam quod! Qui pariatur eaque, omnis exercitationem iusto quidem ex molestias ipsum, unde sequi maiores asperiores quasi ab quia laborum!</div>
  </div>
</template>

<script>
export default {
  components: {}
};
</script>

<style>


.wrapper {

  display: grid;
  grid-template-columns: 1fr;
  grid-auto-rows: auto;




   background-color: rgba(255, 255, 255, 0.75);
  border-radius: 5px;
  box-shadow: 0px 5px 10px rgba(255, 255, 255, 0.75);
  color: #000000;
  padding:20px;
  margin: 10px;
}


.line-1 {
  position: relative;
  top: 50%;
  width: 24em;
  margin: 0 auto;
  border-right: 2px solid rgba(255, 255, 255, 0.75);
  font-size: 180%;
  text-align: center;
  white-space: nowrap;
  overflow: hidden;
  transform: translateY(-50%);
}

/* Animation */
.anim-typewriter {
  animation: typewriter 4s steps(44) 1s 1 normal both,
    blinkTextCursor 500ms steps(44) infinite normal;
}
@keyframes typewriter {
  from {
    width: 0;
  }
  to {
    width: 24em;
  }
}
@keyframes blinkTextCursor {
  from {
    border-right-color: rgba(255, 255, 255, 0.75);
  }
  to {
    border-right-color: transparent;
  }
}
</style>
