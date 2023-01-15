<template>
  <div class="ContactForm">
    <form>
      <input
        type="text"
        v-model="name"
        :class="[nameStatus]"
        placeholder="Name"
      />
      <p class="warning" v-if="nameStatus == 'isFalse'">
        Sorry, this field is required
      </p>
      <input
        type="email"
        v-model="email"
        :class="[emailStatus]"
        placeholder="E-Mail"
      />
      <p class="warning" v-if="emailStatus == 'isFalse'">
        Sorry, invalid format here
      </p>
      <textarea
        type="text"
        v-model="message"
        :class="[messageStatus]"
        placeholder="Message"
      />
      <p class="warning" v-if="messageStatus == 'isFalse'">
        Sorry, this field is required
      </p>
      <button @click.prevent="sendMessage">Send message</button>
    </form>
  </div>
</template>

<script>
export default {
  name: "ContactForm",
  data() {
    return {
      name: "",
      email: "",
      message: "",
      nameStatus: "",
      emailStatus: "",
      messageStatus: "",
    };
  },
  methods: {
    sendMessage() {
      if (this.name && this.validateEmail() && this.message) {
        alert("valid data");
        this.name = "";
        this.email = "";
        this.message = "";
        this.nameStatus = "";
        this.emailStatus = "";
        this.messageStatus = "";
      } else {
        this.validateName();
        this.validateMessage();
        if (this.validateEmail()) {
          this.emailStatus = "isValid";
        } else {
          this.emailStatus = "isFalse";
        }
      }
    },
    validateName() {
      if (this.name) {
        this.nameStatus = "isValid";
      } else {
        this.nameStatus = "isFalse";
      }
    },
    validateEmail() {
      /* eslint-disable */
      if (/^\w+([\.-]?\w+)*@\w+([\.-]?\w+)*(\.\w{2,3})+$/.test(this.email)) {
        return true;
      } else {
        console.log("email is false");
        return false;
      }
    },
    validateMessage() {
      if (this.message) {
        this.messageStatus = "isValid";
      } else {
        this.messageStatus = "isFalse";
      }
    },
  },
};
</script>

<style scoped>
input {
  color: rgba(255, 255, 255, 0.5);
  font-weight: 500;
  font-size: 16px;
  line-height: 26px;
  letter-spacing: -0.222222px;
  mix-blend-mode: normal;
  width: calc(100% - 32px);
  height: 43px;
  margin: 16px 0px;
  padding-left: 24px;
  background-color: transparent;
  border: none;
  border-bottom: 1px solid white;
  text-transform: uppercase;
  outline: none;
}
input:focus {
  color: white;
}

textarea {
  color: rgba(255, 255, 255, 0.5);
  font-weight: 500;
  font-size: 16px;
  line-height: 26px;
  letter-spacing: -0.222222px;
  mix-blend-mode: normal;
  width: calc(100% - 32px);
  height: 43px;
  margin: 16px 0px;
  padding-left: 24px;
  padding-bottom: 80px;
  background-color: transparent;
  border: none;
  border-bottom: 1px solid white;
  text-transform: uppercase;
  outline: none;
}

textarea:focus {
  color: white;
}

.isFalse {
  background: url("../assets/images/warning.png") no-repeat right;
  border-bottom: 1px solid #ff6f5b;
}
.isValid {
  color: white;
  border-bottom: 2px solid green;
}

.warning {
  color: #ff6f5b;
  margin-top: -8px;
  padding-right: 8px;
  text-align: right;
  font-weight: 500;
  font-size: 12px;
  line-height: 16px;
}
</style>
