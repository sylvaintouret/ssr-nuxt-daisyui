<template>
    <div class="flex flex-col border-opacity-50 p-2" style="min-height: 600px;">
        <div class="mockup-code">
            <pre data-prefix="$"><code>login sequence</code></pre> 
            <pre data-prefix=">" class="text-warning"><code>running...</code></pre> 
            <pre data-prefix=">" class="text-success"><code>Done!</code></pre>
        </div>
    </div>
</template>
<script lang="ts" setup>
import { useAuthStore } from '~~/store/auth.store';
const auth = useAuthStore()
auth.login();
</script>