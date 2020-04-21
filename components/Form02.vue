<template>
  <div class="contact">
    <p class="title is-5">
      Form02の説明だよ〜
    </p>
    <form
      name="Form02"
      action="/success"
      method="post"
      data-netlify="true"
      data-netlify-honeypot="bot-field"
      class="form"
    >
      <input type="hidden" name="form-name" value="Form02" />
      <div class="block">
        <label class="label">御社名</label
        ><input type="text" name="companyName" class="input" />
      </div>
      <div class="block">
        <label class="label">ご担当者様名</label
        ><input type="text" name="name" class="input" />
      </div>
      <div class="block">
        <label class="label">ご連絡先電話番号</label
        ><input type="tel" name="tel" class="input" />
      </div>
      <div class="block">
        <label class="label">メールアドレス</label
        ><input type="email" name="email" class="input" />
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
