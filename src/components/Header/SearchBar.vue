<template>
  <div class="search-bar">
    <div class="search-icon">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 56.966 56.966"
        fill="%23717790c7"
      >
        <path
          d="M55.146 51.887L41.588 37.786A22.926 22.926 0 0046.984 23c0-12.682-10.318-23-23-23s-23 10.318-23 23 10.318 23 23 23c4.761 0 9.298-1.436 13.177-4.162l13.661 14.208c.571.593 1.339.92 2.162.92.779 0 1.518-.297 2.079-.837a3.004 3.004 0 00.083-4.242zM23.984 6c9.374 0 17 7.626 17 17s-7.626 17-17 17-17-7.626-17-17 7.626-17 17-17z"
        />
      </svg>
    </div>
    <input type="text" placeholder="Search" />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  setup() {
    return {};
  },
});
</script>

<style lang="scss">
.search-bar {
  height: calc(100% - 18px);
  display: flex;
  width: 100%;
  max-width: 400px;
  padding: 0 16px;
  border-radius: 4px;
  position: relative;
  .search-icon {
    position: absolute;
    width: 40px;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    svg {
      height: 1em;
      fill: var(--inactive-color);
    }
  }
  input {
    width: 100%;
    height: 100%;
    border: none;
    background-color: var(--theme-deep-color);
    border-radius: 4px;
    font-size: 15px;
    font-weight: 500;
    padding: 0 20px 0 40px;
    box-shadow: 0 0 0 2px var(--border-color);
    color: var(--theme-color);
    &::placeholder {
      color: var(--inactive-color);
      font-size: 15px;
      font-weight: 500;
    }
  }
}
</style>
