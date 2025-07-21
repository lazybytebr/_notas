# ✅ Resumo de PHP: Tabelas de Estudo

---

## 📦 Tipos de Dados no PHP 8

| Tipo de Dado        | Explicação Curta                                                               | Exemplo                                |
|---------------------|--------------------------------------------------------------------------------|----------------------------------------|
| `int`               | Número inteiro, positivo ou negativo.                                          | `<?php $idade = 30; ?>`                |
| `float`             | Número com casas decimais.                                                     | `<?php $preco = 99.90; ?>`             |
| `string`            | Sequência de caracteres.                                                       | `<?php $nome = "Alberto"; ?>`         |
| `bool`              | Valor lógico: `true` ou `false`.                                               | `<?php $ativo = true; ?>`             |
| `array`             | Conjunto de valores indexados.                                                 | `<?php $frutas = ["maçã", "banana"]; ?>` |
| `object`            | Instância de uma classe.                                                       | `<?php class Pessoa {} $p = new Pessoa(); ?>` |
| `null`              | Representa ausência de valor.                                                  | `<?php $x = null; ?>`                 |
| `resource`          | Referência a recursos externos (ex: arquivo).                                  | `<?php $f = fopen("file.txt", "r"); ?>` |
| `mixed`             | Pode ser qualquer tipo de dado.                                                | `<?php function test(mixed $v) {} ?>` |
| `callable`          | Função/método que pode ser chamado.                                            | `<?php $f = function() {}; $f(); ?>`  |
| `iterable`          | Pode ser percorrido com `foreach`.                                             | `<?php function get(): iterable { return [1]; } ?>` |
| `never` (PHP 8.1+)  | Indica que a função nunca retorna (ex: `exit()`).                              | `<?php function erro(): never { exit(); } ?>` |

---

## 🔀 Condicionais em PHP

| Condicional   | Explicação Curta                                         | Exemplo                                                        |
|---------------|----------------------------------------------------------|----------------------------------------------------------------|
| `if`          | Executa se a condição for verdadeira.                    | `if ($idade >= 18) { echo "Maior"; }`                         |
| `else`        | Executa se a condição do `if` for falsa.                 | `if ($idade >= 18) { ... } else { echo "Menor"; }`            |
| `elseif`      | Verifica outra condição se a anterior for falsa.         | `if ($n < 0) {} elseif ($n == 0) {}`                          |
| `switch`      | Compara uma variável com vários casos.                   | `switch ($dia) { case "seg": echo "Segunda"; break; }`       |
| `match` (8+)  | Versão moderna do `switch`, retorna valor diretamente.   | `$msg = match($dia) { "seg" => "Segunda", default => "Outro" };` |
| Ternário `? :`| Condição compacta em uma linha.                          | `echo ($idade >= 18) ? "Maior" : "Menor";`                    |
| Null coalescing `??` | Retorna o valor se não for nulo.                         | `$nome = $_GET["nome"] ?? "Visitante";`                       |

---

## 🔁 Laços de Repetição

| Laço         | Explicação Curta                                         | Exemplo                                      |
|--------------|----------------------------------------------------------|----------------------------------------------|
| `for`        | Repete com contador.                                     | `for ($i = 0; $i < 5; $i++) { echo $i; }`   |
| `while`      | Executa enquanto for verdadeiro.                         | `$i = 0; while ($i < 5) { echo $i++; }`     |
| `do...while` | Executa pelo menos uma vez.                              | `$i = 0; do { echo $i++; } while ($i < 5);` |
| `foreach`    | Percorre elementos de array.                             | `foreach ($lista as $item) { echo $item; }`|
| `break`      | Encerra o loop atual.                                    | `if ($i == 3) break;`                        |
| `continue`   | Pula para próxima iteração.                              | `if ($i == 2) continue;`                     |

---

## 🔣 Operadores Lógicos

| Operador | Nome               | Explicação Curta                                     | Exemplo                                      |
|----------|--------------------|------------------------------------------------------|----------------------------------------------|
| `&&`     | E lógico           | Verdadeiro se ambas forem verdadeiras.              | `if ($a > 0 && $b > 0)`                      |
| `and`    | E lógico (baixa precedência) | Igual ao `&&`, mas com precedência menor.           | `if ($a > 0 and $b > 0)`                     |
| `||`     | OU lógico          | Verdadeiro se ao menos uma for verdadeira.          | `if ($a > 0 || $b > 0)`                      |
| `or`     | OU lógico (baixa precedência) | Igual ao `||`, mas com precedência menor.           | `if ($a > 0 or $b > 0)`                      |
| `!`      | NÃO lógico         | Inverte o valor lógico.                             | `if (!empty($x))`                            |
| `xor`    | OU exclusivo       | Verdadeiro se **apenas uma** for verdadeira.        | `if ($a xor $b)`                             |

---

## ➕ Operadores Aritméticos

| Operador | Nome           | Explicação Curta                     | Exemplo           |
|----------|----------------|--------------------------------------|-------------------|
| `+`      | Adição         | Soma dois valores.                   | `5 + 3 // 8`       |
| `-`      | Subtração      | Subtrai o segundo do primeiro.       | `5 - 2 // 3`       |
| `*`      | Multiplicação  | Multiplica dois valores.             | `4 * 2 // 8`       |
| `/`      | Divisão        | Divide o primeiro pelo segundo.      | `10 / 2 // 5`      |
| `%`      | Módulo         | Resto da divisão.                    | `10 % 3 // 1`      |
| `**`     | Exponenciação  | Eleva à potência.                    | `2 ** 3 // 8`      |

---

## 📝 Operadores de Atribuição

| Operador | Nome                 | Explicação Curta                          | Exemplo               |
|----------|----------------------|-------------------------------------------|------------------------|
| `=`      | Atribuição           | Define valor da variável.                 | `$x = 10;`             |
| `+=`     | Soma e atribui       | Soma e salva na mesma variável.           | `$x += 5;`             |
| `-=`     | Subtrai e atribui    | Subtrai e atualiza a variável.            | `$x -= 2;`             |
| `*=`     | Multiplica e atribui | Multiplica e atualiza a variável.         | `$x *= 3;`             |
| `/=`     | Divide e atribui     | Divide e atualiza a variável.             | `$x /= 2;`             |
| `%=`     | Módulo e atribui     | Aplica módulo e atualiza.                 | `$x %= 4;`             |
| `**=`    | Potência e atribui   | Eleva e atualiza.                         | `$x **= 2;`            |

---

## ⚙️ Funções Built-in (principais)

### 🔤 Manipulação de Strings

| Função         | Explicação Curta                   | Exemplo                        |
|----------------|------------------------------------|--------------------------------|
| `strlen()`     | Conta caracteres.                  | `strlen("PHP") // 3`           |
| `strtoupper()` | Converte para maiúsculas.          | `strtoupper("php")`            |
| `strtolower()` | Converte para minúsculas.          | `strtolower("PHP")`            |
| `substr()`     | Retorna parte da string.           | `substr("abc", 1, 2) // "bc"`  |
| `str_replace()`| Substitui na string.               | `str_replace("mundo", "PHP", "Olá mundo")` |
| `trim()`       | Remove espaços nas bordas.         | `trim("  oi ") // "oi"`        |

### 🔢 Números

| Função     | Explicação Curta               | Exemplo        |
|------------|--------------------------------|----------------|
| `abs()`    | Valor absoluto.                | `abs(-10)`     |
| `round()`  | Arredonda.                     | `round(3.6)`   |
| `floor()`  | Arredonda para baixo.          | `floor(3.9)`   |
| `ceil()`   | Arredonda para cima.           | `ceil(3.1)`    |
| `rand()`   | Número aleatório.              | `rand(1, 100)` |

### 📚 Arrays

| Função         | Explicação Curta                    | Exemplo                         |
|----------------|-------------------------------------|----------------------------------|
| `count()`      | Conta elementos do array.           | `count([1,2,3]) // 3`            |
| `array_merge()`| Junta arrays.                       | `array_merge([1],[2])`          |
| `in_array()`   | Verifica valor no array.            | `in_array(2, [1,2,3])`          |
| `array_keys()` | Retorna chaves do array.            | `array_keys(['a'=>1])`          |
| `array_values()`| Retorna apenas os valores.         | `array_values(['a'=>1])`        |

---

## 📁 move_uploaded_file()

| Item                | Descrição                                                                  |
|---------------------|---------------------------------------------------------------------------|
| Nome                | `move_uploaded_file()`                                                     |
| Função              | Move um arquivo enviado via formulário para outro local.                   |
| Parâmetros          | `move_uploaded_file($tmp, $destino)`                                       |
| Retorno             | `true` se mover com sucesso, `false` se falhar.                            |
| Uso comum           | Após upload com `enctype="multipart/form-data"`.                           |
| Validação           | Só funciona com arquivos válidos enviados via `POST`.                      |

### Exemplo:

```php
if (isset($_FILES['arquivo'])) {
    $tmp = $_FILES['arquivo']['tmp_name'];
    $destino = "uploads/" . $_FILES['arquivo']['name'];

    if (move_uploaded_file($tmp, $destino)) {
        echo "Upload ok!";
    } else {
        echo "Erro no upload.";
    }
}
