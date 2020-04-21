<template>
  <div class="contact">
    <p class="title is-5">
      Form01の説明だよ〜
    </p>
    <form
      name="Form01"
      action="/success"
      method="post"
      data-netlify="true"
      data-netlify-honeypot="bot-field"
      class="form"
    >
      <input type="hidden" name="form-name" value="Form01" />
      <div class="block">
        <label class="label">お名前</label
        ><input type="text" name="name" class="input" />
      </div>
      <div class="block">
        <label class="label">ご連絡先メールアドレス、電話番号）</label
        ><input type="text" name="email" class="input" />
      </div>
      <div class="block">
        <label class="label">お問い合わせ内容</label
        ><textarea name="message" class="input" />
      </div>
      <button class="button">
        送信する
      </button>
    </form>
  </div>
</template>

<script>
export default {}
</script>
