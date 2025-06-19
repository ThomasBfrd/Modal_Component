# React Modal Component

A simple, customizable React modal component built with Typescript

![SASS](https://img.shields.io/badge/SASS-hotpink.svg?style=for-the-badge&logo=SASS&logoColor=white)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![Vite](https://img.shields.io/badge/vite-%23646CFF.svg?style=for-the-badge&logo=vite&logoColor=white)
![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)

## Installation
In your project, just copy and paste this line :
```
npm i @thomasbfrd/modal
```

## Features

- **Success Modal**: Displays a success message with a single confirmation button
- **Error Modal**: Shows error messages with a close button
- **Submit Modal**: Confirmation dialog with both confirm and cancel options


## Usage
```
type: 'success' | 'error' | 'submit'
title: string;
body: string;
cancelButton?: string;
okButton: string;
onCancel?: () => void;
onOk: () => void;
```

### Importation : <br>
```
import { Modal } from "@thomasbfrd/modal";
import "@thomasbfrd/modal/dist/modal.css";
```

```
Success Modal 
<Modal 
    type="success" 
    title="Success!" 
    body="Operation completed successfully" 
    okButton="Close" 
    onOk={() => {}} 
/>

Error Modal 
<Modal 
    type="error" 
    title="Error" 
    body="Something went wrong" 
    okButton="Close" 
    onOk={() => {}} 
/>

Submit Modal (with confirmation) 
<Modal 
    type="submit" 
    title="Confirm" 
    body="Are you sure?" 
    okButton="Confirm" 
    cancelButton="Cancel" 
    onOk={() => {}} 
    onCancel={() => {}} 
/>
```

### Customization
```
:root { 
    --modal-background-color: #1E293B; 
    --modal-primary-color: #F8FAFC; 
    --modal-secondary-color: #1E293B; 
    --modal-button-primary-color: #1e1e1e; 
    --modal-button-secondary-color: #1E293B; 
}
```

## Demo

![ModalDemo](https://i.postimg.cc/R066D42z/modal-demo.png)
