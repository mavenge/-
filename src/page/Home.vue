<template>
  <div class="home">
    <img src="../assets/1_画板 1.jpg" />
    <div class="filter">
      <div class="blur"></div>
    </div>
    <div class="content">
      <div class="stone">
        <img class="village" src="../assets/village/1.png" alt="stone">
        <img class="board" src="../assets/guideboard/1.png" alt="board">
        <img class="brick" src="../assets/brick/1.png" alt="brick">
        <img class="decorate" src="../assets/decorate/1.png" alt="decorate">
      </div>

      <div class="daliangjiang">
        <img class="village" src="../assets/village/2.png" alt="stone">
        <img class="board" src="../assets/guideboard/2.png" alt="board">
        <img class="brick" src="../assets/brick/2.png" alt="brick">
      </div>

      <div class="lvjia">
        <img class="village" src="../assets/village/3.png" alt="stone">
        <img class="board" src="../assets/guideboard/3.png" alt="board">
        <img class="brick" src="../assets/brick/3.png" alt="brick">
        <img class="decorate" src="../assets/decorate/2.png" alt="stone">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
};
</script>

<style scoped lang="less">
.home {
  width: 100vw;
  background: radial-gradient(#abbfc0, #ccd6d5);

  img {
    width: 100%;
  }

  .filter {
    position: relative;

    .blur {
      height: 10px;
      width: 100vw;
      background-color: #abbfc0;
      filter: blur(5px);
      position: absolute;
      top: -3px;
      left: 0;
    }
  }

  .content {
    .stone {
      height: 500px;
      position: relative;

      .village {
        width: 250px;
        position: absolute;
        right: 0;
      }

      .board {
        width: 100px;
        position: absolute;
        top: 150px;
        left: 60px;
      }

      .brick {
        width: 200px;
        position: absolute;
        top: 190px;
        left: 80px;
      }

      .decorate {
        width: 100px;
        position: absolute;
        top: 200px;
        right: 40px;
      }

    }

    .daliangjiang {
      height: 200px;
      position: relative;

      .village {
        width: 250px;
        position: absolute;
        left: 0;
        top: -120px;
        z-index: 2;
      }

      .board {
        width: 100px;
        position: absolute;
        top: -40px;
        right: 80px;
        z-index: 3;
      }

      .brick {
        width: 200px;
        position: absolute;
        top: -40px;
        left: 60px;
      }

    }

    .lvjia {
      height: 500px;
      position: relative;

      .village {
        width: 300px;
        position: absolute;
        right: 0;
      }

      .board {
        width: 100px;
        position: absolute;
        top: 150px;
        left: 60px;
      }

      .brick {
        width: 250px;
        position: absolute;
        top: 150px;
        left: 80px;
      }

      .decorate {
        width: 160px;
        position: absolute;
        top: 200px;
        left: 40px;
      }
    }

  }


}
</style>