<script setup>
import GuestLayOut from "@/Layouts/GuestLayout.vue";
import Label from "@/Components/InputLabel.vue";
import Input from "@/Components/TextInput.vue";

const emitTest = (e) => console.log(e);
</script>

<template>
    <GuestLayOut>
        <Label value="件名">タイトル </Label>
        <Input
            modelValue="初期値が入ります"
            @update:modelValue="emitTest"
        ></Input>
    </GuestLayOut>
</template>
