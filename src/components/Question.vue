<template>
  <div class="my-wrapper">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <h1>Здесь будет название вопроса?</h1>
          <hr>
          <div class="answers">
            <form>
              <div class="custom-control custom-checkbox">
                <input type="checkbox" class="custom-control-input" id="customCheck1">
                <label class="custom-control-label" for="customCheck1">Вариант ответа 1</label>
              </div>
              <hr>
              <button type="submit" class="btn btn-success">Далее</button>
            </form>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'Question',
  props: ['func', 'getQuests'],
  data() {
    return {}
  }
}
</script>
<style scoped>
.my-wrapper {
  margin-top: 50px;
}

.answers {
  margin-top: 50px;
}
</style>