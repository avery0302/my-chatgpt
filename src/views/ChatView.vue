<template>
  <div class="container">
    <div class="left">
      <div class="favicon">
        <img alt="site icon" src="../assets/icon.png" />
      </div>
      <div class="sidebar">
        <div class="item">
          <i class="pi pi-pen-to-square"></i>
        </div>
        <div class="item">
          <i class="pi pi-search"></i>
        </div>
        <div class="item">
          <i class="pi pi-images"></i>
        </div>
      </div>
      <div class="user">
        <div class="round">
          <div class="round-border bd">
            <i class="pi pi-user"></i>
          </div>
        </div>
      </div>
    </div>
    <div class="right">
      <div class="header">
        <div class="model">
          <div class="text">ChatGPT</div>
          <i class="pi pi-angle-down"></i>
        </div>
        <div class="header-right">
          <div class="free">
            <i class="pi pi-gift"></i>
            <div>Free offer</div>
          </div>
          <div class="share">
            <i class="pi pi-upload"></i>
            <div>Share</div>
          </div>
          <div class="more">
            <i class="pi pi-ellipsis-h"></i>
          </div>
        </div>
      </div>
      <div class="chat">
        <div class="dev">Under Development</div>
        <div class="input-area">
          <div class="input-box">
            <div class="button-box">
              <Button
                iconOnly
                variant="text"
                severity="contrast"
                aria-label="add"
              >
                <i class="pi pi-plus"></i>
              </Button>
            </div>
            <InputText placeholder="Ask anything" />
            <div class="button-box">
              <Button
                iconOnly
                variant="text"
                severity="contrast"
                aria-label="voice"
              >
                <i class="pi pi-microphone mic"></i>
              </Button>
            </div>
            <div class="button-box">
              <Button iconOnly severity="contrast" aria-label="send">
                <i class="pi pi-headphones"></i>
              </Button>
            </div>
          </div>
        </div>
        <div class="tip">ChatGPT can make mistakes. Check important info.</div>
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
    width: 55px;
    display: flex;
    flex-direction: column;
    background: rgb(245, 245, 245);
    border-right: 1px solid rgb(230, 230, 230);

    .favicon {
      height: 60px;
      display: flex;
      align-items: center;
      justify-content: center;

      img {
        height: 30px;
      }
    }

    .sidebar {
      flex: 1;

      .item {
        height: 35px;
        display: flex;
        align-items: center;
        justify-content: center;
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

        .round-border {
          border-radius: 50%;
          height: 13px;
          width: 13px;
          display: flex;
          align-items: center;
          justify-content: center;
        }

        i {
          font-size: 9px;
        }
      }
    }
  }

  .right {
    flex: 1;
    display: flex;
    flex-direction: column;
    background: rgb(249, 249, 249);

    .header {
      margin: 0 15px;
      height: 55px;
      display: flex;
      border-bottom: 1px solid rgb(230, 230, 230);

      .model {
        width: 130px;
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 4px;

        .text {
          font-size: 18px;
          font-weight: 600;
        }

        i {
          color: rgb(147, 147, 147);
        }
      }

      .header-right {
        flex: 1;
        display: flex;
        justify-content: end;
        font-size: 14px;

        .free {
          width: 125px;
          display: flex;
          align-items: center;
          justify-content: center;
          gap: 8px;
          color: rgb(0, 109, 186);

          i {
            font-size: 16px;
          }
        }

        .share {
          width: 75px;
          display: flex;
          align-items: center;
          justify-content: center;
          gap: 8px;

          i {
            font-size: 15px;
          }
        }

        .more {
          width: 50px;
          display: flex;
          align-items: center;
          justify-content: center;
        }
      }
    }

    .chat {
      flex: 1;
      display: flex;
      flex-direction: column;
      justify-content: end;

      .dev {
        flex: 1;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 60px;
      }

      .input-area {
        height: 55px;
        display: flex;
        align-items: center;
        justify-content: center;

        .input-box {
          width: 65%;
          height: 54px;
          border-radius: 27px;
          border: 1px solid rgb(226, 226, 226);
          display: flex;
          background: white;

          input {
            flex: 1;
            border: none;
            padding: 0;

            &::placeholder {
              color: rgb(150, 150, 150);
            }
          }

          .button-box {
            width: 50px;
            height: 50px;
            display: flex;
            align-items: center;
            justify-content: center;

            button {
              width: 35px;
              height: 35px;
              border-radius: 50%;

              .mic {
                font-size: 20px;
              }
            }
          }
        }
      }

      .tip {
        display: flex;
        align-items: center;
        justify-content: center;
        height: 35px;
        font-size: 12px;
        color: rgb(157, 157, 157);
      }
    }
  }
}
</style>
