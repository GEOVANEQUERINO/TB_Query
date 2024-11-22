# Estrutura das Tabelas

### Tabela: `provas`
| **Coluna**         | **Tipo**          |
|---------------------|-------------------|
| `id_aluno`         | número           |
| `id_materia`       | número           |
| `nota`             | número flutuante |
| `data_da_prova`    | data             |

---

### Tabela: `aluno`
| **Coluna**         | **Tipo**  |
|---------------------|-----------|
| `id`               | número    |
| `nome`             | string    |
| `data_nascimento`  | número    |

---

### Tabela: `professor`
| **Coluna**         | **Tipo**  |
|---------------------|-----------|
| `id`               | número    |
| `nome`             | string    |
| `data_nascimento`  | número    |

---

### Tabela: `materia`
| **Coluna**         | **Tipo**  |
|---------------------|-----------|
| `id`               | número    |
| `nome`             | string    |
| `id_professor`     | número    |

---

## Queries pedidas

### 1. Inserir Alunos
INSERT INTO aluno (id, nome, data_nascimento) VALUES
(1, 'João Silva', '2005-03-10'),
(2, 'Maria Souza', '2006-07-15'),
(3, 'Carlos Almeida', '2004-12-22');

### 2. Inserir Professor
INSERT INTO professor (id, nome, data_nascimento) VALUES
(1, 'Ana Ribeiro', '1980-05-14');

### 3. Inserir Matéria
INSERT INTO materia (id, nome, id_professor) VALUES
(1, 'Matemática', 1);

### 4. Inserir Provas e Notas
INSERT INTO provas (id_aluno, id_materia, nota, data_da_prova) VALUES
(1, 1, 8.5, '2024-11-20'),
(2, 1, 9.0, '2024-11-20'),
(3, 1, 7.5, '2024-11-20');



