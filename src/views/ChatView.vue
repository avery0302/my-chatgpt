<template>
  <div class="container">
    <div class="bg left">
      <div class="bd favicon">1</div>
      <div class="sidebar">
        <div class="bd item">2</div>
        <div class="bd item">3</div>
        <div class="bd item">4</div>
      </div>
      <div class="bd user">
        <div class="bd round">
          <i class="pi pi-user"></i>
        </div>
      </div>
    </div>
    <div class="right">
      <div class="bd header">
        <div class="model bd">5</div>
        <div class="header-right">
          <div class="free bd">6</div>
          <div class="share bd">7</div>
          <div class="more">8</div>
        </div>
      </div>
      <div class="bd chat">
        <div class="bd input">9</div>
        <div class="bd tip">ChatGPT也可能会犯错。请核查重要信息。</div>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style scoped>
.container {
  display: flex;
  height: 100%;

  .left {
    width: 50px;
    display: flex;
    flex-direction: column;

    .favicon {
      height: 55px;
    }

    .sidebar {
      flex: 1;

      .item {
        height: 35px;
      }
    }

    .user {
      height: 70px;
      display: flex;
      align-items: center;
      justify-content: center;

      .round {
        background: rgb(229, 229, 229);
        height: 25px;
        width: 25px;
        display: flex;
        align-items: center;
        justify-content: center;
        border-radius: 50%;

        i {
          font-size: 12px;
        }
      }
    }
  }

  .right {
    flex: 1;
    display: flex;
    flex-direction: column;

    .header {
      height: 55px;
      display: flex;

      .model {
        width: 155px;
      }

      .header-right {
        flex: 1;
        display: flex;
        justify-content: end;

        .free {
          width: 95px;
        }

        .share {
          width: 75px;
        }

        .more {
          width: 55px;
        }
      }
    }

    .chat {
      flex: 1;
      display: flex;
      flex-direction: column;
      justify-content: end;

      .input {
        height: 55px;
      }

      .tip {
        display: flex;
        justify-content: center;
        height: 35px;
        font-size: 12.5px;
        color: rgb(157, 157, 157);
      }
    }
  }
}
</style>
