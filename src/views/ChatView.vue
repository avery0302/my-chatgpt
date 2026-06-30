<template>
  <div class="container">
    <div class="bg left">
      <div class="bg-red favicon">111</div>
      <div class="sidebar">
        <div class="bg-yellow item">4</div>
        <div class="bg-red item">5</div>
        <div class="bg-green item">6</div>
      </div>
      <div class="bg-green user">333</div>
    </div>
    <div class="right">
      <div class="bg-yellow header">
        <div class="model bg-red">1</div>
        <div class="header-right">
          <div class="free bg-green">2</div>
          <div class="share bg-red">3</div>
          <div class="more">4</div>
        </div>
      </div>
      <div class="bg-blue chat">
        <div class="bg-red input">111</div>
        <div class="bg-yellow tip">ChatGPT也可能会犯错。请核查重要信息。</div>
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
      height: 60px;
    }

    .sidebar {
      flex: 1;

      .item {
        height: 35px;
      }
    }

    .user {
      height: 70px;
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
      }
    }
  }
}
</style>
