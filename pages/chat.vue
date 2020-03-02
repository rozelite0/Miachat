<template>
  <div class="container">
    <div class="info">
      <img class="friend-icon" src="http://placehold.jp/80x80.png" />
      <h2 class="friend-name">相手の名前</h2>
    </div>

    <div class="chat">
      <div class="friend-balloon">
        <div class="balloon-left">
          <p>
            左吹き出し
            <br />これは今日無論その観念人というののところを進んだらしく。依然として先刻に諷刺人はとにかくその評るないまでを来てしまえたにも努力するですなし、これからには考えないでですう。気となりたのはもし事実によくませならまし。いったん岡田さんに記憶時分わざわざ安心に云うなけれ願その義務そちらか講演からによってご応用たですででて、このほかは私かその道長靴に認めて、大森さんののに一般のそれにせっかくお乱暴と見てそれ人をご出立と伺いようにどうしてもご永続へ違っなないから、あたかもずっと意味に亡びならからくるべき方によるまします。ただかつお政府にあっものはそうむやみと乗っなけれて、この主義にも知れですからとして事情をなるて来うなら。
          </p>
        </div>
      </div>

      <div class="user-balloon">
        <div class="balloon-right">
          <p>これは今日無論その観念人というののところを進んだらしく。依然として先刻に諷刺人はとにかくその評るないまでを来てしまえたにも努力するですなし、これからには考えないでですう。気となりたのはもし事実によくませならまし。いったん岡田さんに記憶時分わざわざ安心に云うなけれ願その義務そちらか講演からによってご応用たですででて、このほかは私かその道長靴に認めて、大森さんののに一般のそれにせっかくお乱暴と見てそれ人をご出立と伺いようにどうしてもご永続へ違っなないから、あたかもずっと意味に亡びならからくるべき方によるまします。ただかつお政府にあっものはそうむやみと乗っなけれて、この主義にも知れですからとして事情をなるて来うなら。</p>
        </div>
      </div>

      <div class="friend-balloon">
        <div class="balloon-left">
          <p>左吹き出し</p>
        </div>
      </div>

      <div class="friend-balloon">
        <div class="balloon-left">
          <p>左吹き出し</p>
        </div>
      </div>

      <div class="user-balloon">
        <div class="balloon-right">
          <p>そっか</p>
        </div>
      </div>

    </div>

    <div class="input-field">
      <form>
        <textarea name id cols="140" rows="5"></textarea>
      </form>
      <div class="stamp-menu"></div>
    </div>
  </div>
</template>

<script>
import Logo from "~/components/Logo.vue";

export default {
  components: {
    Logo
  }
};
</script>

<style>
.info {
  background-color: #555;
  height: 120px;
}

.friend-icon {
  margin: 20px;
  float: left;
  border-radius: 50%;
}

.chat {
  width: 80%;
  height: 70vh;
  margin: 0 auto;
  padding: 30px;
  overflow-x: hidden;
  overflow-y: scroll;
}

.balloon-left {
  clear: both;
  position: relative;
  display: inline-block;
  margin: 10px auto 10px 15px;
  padding: 7px 10px;
  min-width: 120px;
  max-width: 100%;
  color: #555;
  font-size: 16px;
  background: #fff;
  border: solid 3px #555;
  box-sizing: border-box;
}

.balloon-left:before {
  content: "";
  position: absolute;
  top: 50%;
  left: -24px;
  margin-top: -12px;
  border: 12px solid transparent;
  border-right: 12px solid #fff;
  z-index: 2;
}

.balloon-left:after {
  content: "";
  position: absolute;
  top: 50%;
  left: -30px;
  margin-top: -14px;
  border: 14px solid transparent;
  border-right: 14px solid #555;
  z-index: 1;
}

.balloon-right {
  position: relative;
  display: inline-block;
  padding: 7px 10px;
  margin: 10px auto 10px 15px;
  min-width: 120px;
  max-width: 100%;
  color: #555;
  font-size: 16px;
  background: #fff;
  border: solid 3px #555;
  box-sizing: border-box;
}

.balloon-right:before {
  content: "";
  position: absolute;
  top: 50%;
  right: -24px;
  margin-top: -12px;
  border: 12px solid transparent;
  border-left: 12px solid #fff;
  z-index: 2;
}

.balloon-right:after {
  content: "";
  position: absolute;
  top: 50%;
  right: -30px;
  margin-top: -14px;
  border: 14px solid transparent;
  border-left: 14px solid #555;
  z-index: 1;
}

.balloon-right p {
  margin: 0;
  padding: 0;
}

.user-balloon {
}

.friend-name {
  color: #fff;
  position: relative;
  top: 40px;
}

.input-field {
  margin: 0;
  padding: 10px;
  background: #35495e;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
