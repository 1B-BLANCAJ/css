# css
:root {
    --purple: #4840d2;
    --navy: #22263f;
    --field: #4a4b5d;
    --green: #8bc77f;
}

* {
    box-sizing: border-box;
}

body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: var(--navy);
    color: white;
}

header {
    background: var(--purple);
    padding: 20px;
    display: flex;
    align-items: center;
    gap: 12px;
    min-height: 135px;
}

.logo {
    font-size: 55px;
}

.brand h1 {
    font-size: clamp(20px, 4vw, 34px);
    line-height: 1.08;
    margin: 0;
}

.brand p {
    font-size: clamp(12px, 2.5vw, 20px);
    margin: 8px 0 0;
}

nav {
    background: #f7f6f2;
    display: flex;
    justify-content: space-around;
    align-items: center;
    padding: 10px 4px;
    gap: 4px;
}

nav button {
    background: transparent;
    color: var(--green);
    border: 0;
    padding: 10px 6px;
    font-size: clamp(13px, 2.5vw, 24px);
    display: flex;
    align-items: center;
    gap: 6px;
    cursor: pointer;
}

nav button.active {
    background: #e6f1e3;
    border-radius: 10px;
    color: #4b9945;
}

.icon {
    font-size: clamp(23px, 4vw, 40px);
}

main {
    max-width: 850px;
    margin: auto;
    padding: 22px 22px 60px;
}

.page {
    display: none;
}

.page.active {
    display: block;
}

h2 {
    text-align: center;
    font-size: clamp(27px, 5vw, 40px);
    margin: 25px 0 42px;
}

.field {
    margin-bottom: 27px;
}

label {
    display: block;
    font-size: clamp(18px, 3vw, 25px);
    font-weight: bold;
    margin: 0 0 12px 8px;
}

input,
select {
    width: 100%;
    min-height: 60px;
    padding: 16px 25px;
    border: 2px solid transparent;
    border-radius: 32px;
    background: var(--field);
    color: white;
    font-size: clamp(16px, 2.5vw, 22px);
    outline: none;
}

input::placeholder {
    color: #eee;
    opacity: 1;
}

input:focus,
select:focus {
    border-color: #aaa6ff;
}

.primary {
    display: block;
    margin: 32px auto 0;
    padding: 18px 28px;
    min-width: 220px;
    border: 0;
    border-radius: 28px;
    background: var(--field);
    color: white;
    font-size: clamp(21px, 3.5vw, 30px);
    font-weight: bold;
    cursor: pointer;
}

.primary:hover {
    background: #62647b;
}

.note {
    text-align: center;
    color: #dddff0;
    font-size: 14px;
    line-height: 1.5;
}

.message {
    display: none;
    margin: 18px auto;
    padding: 13px;
    border-radius: 12px;
    text-align: center;
    line-height: 1.4;
}

.error {
    display: block;
    background: #5b2e3b;
}

.success {
    display: block;
    background: #244d3b;
}

.loginbox {
    max-width: 620px;
    margin: auto;
    padding-top: clamp(40px, 10vw, 100px);
}

.loginbox .field {
    margin-bottom: 38px;
}

.loginbox .primary {
    margin-top: 60px;
}

.panel {
    background: #2c304a;
    border: 1px solid #454a68;
    border-radius: 16px;
    padding: 18px;
    margin: 18px 0;
}

.stats {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 8px;
}

.stat {
    text-align: center;
    background: var(--field);
    border-radius: 12px;
    padding: 14px 5px;
}

.stat strong {
    display: block;
    font-size: 24px;
}

.stat span {
    font-size: 13px;
    color: #eee;
}

.tablewrap {
    overflow-x: auto;
}

table {
    width: 100%;
    min-width: 560px;
    border-collapse: collapse;
    margin-top: 15px;
}

td,
th {
    text-align: left;
    padding: 10px;
    border-bottom: 1px solid #50546e;
    font-size: 13px;
}

th {
    color: #bde9b3;
}

.small {
    background: #6a3440;
    border: 0;
    border-radius: 8px;
    padding: 10px;
    color: white;
    cursor: pointer;
}

.logout {
    font-size: 20px;
    min-width: 0;
}

@media (max-width: 520px) {
    header {
        padding: 16px 12px;
        gap: 8px;
    }

    .logo {
        font-size: 42px;
    }

    nav button {
        font-size: 12px;
        gap: 3px;
        padding: 8px 3px;
    }

    .icon {
        font-size: 23px;
    }

    main {
        padding: 18px 17px 45px;
    }

    .stats {
        gap: 5px;
    }

    .stat strong {
        font-size: 20px;
    }

    .stat span {
        font-size: 11px;
    }
}
