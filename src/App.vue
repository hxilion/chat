<script setup lang="ts">
import { TUIKit } from "./TUIKit";
import { TUICallKit } from "@tencentcloud/call-uikit-vue";
import { TUITranslateService } from "@tencentcloud/chat-uikit-engine";
import { TUIUserService } from "@tencentcloud/chat-uikit-engine";

TUITranslateService.changeLanguage("zh");
TUIUserService.switchMessageReadStatus(true); // 开启
</script>

<template>
  <div>
    <TUIKit
      :SDKAppID="20014661"
      userID="lion"
      userSig="eJyrVgrxCdYrSy1SslIy0jNQ0gHzM1NS80oy0zLBwjmZ*XlQ8eKU7MSCgswUJSsjAwNDEzMzQ4h4akVBZlGqkpWhqakpUMYAIlqSmQsSMzc2MjI1Nje1hJqRmQ401N2tNL0ytTwqKlHbIMTbPUbfx8-c281Eu8C5uNJC2zzVz6*oyNUzwN88pCjZVqkWAMHSMFY_"
    />
    <TUICallKit
      class="callkit-container"
      :allowedMinimized="true"
      :allowedFullScreen="false"
    />
  </div>
</template>

<style lang="scss" scoped></style>
