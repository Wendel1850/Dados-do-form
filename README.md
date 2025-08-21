# Dados-do-form
import React, { useState } from 'react';

const Form = () => {
  const [nome, setNome] = useState('');
  const [email, setEmail] = useState('');
  const [mensagem, setMensagem] = useState('');

  const handleSubmit = (event) => {
    event.preventDefault();
    const dados = {
      nome,
      email,
      mensagem
    };
    console.log(dados);
  };

  return (
    <form onSubmit={handleSubmit}>
      <label>Nome:</label>
      <input type="text" value
      
