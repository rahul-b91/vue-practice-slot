<template>
  <div>
    <slot>fallback content in case of not any content is comming</slot>

    <slot name="second"></slot>

    <slot name="third"></slot>
  </div>
</template>