<template>
    <div id="login-template">
        <div>
            <input type="text" placeholder="ログインID" v-model="userid">
        </div>
        <div>
            <input type="password" placeholder="パスワード" v-model="password">
        </div>
        <button @click="login">ログイン</button>
    </div>
</template>