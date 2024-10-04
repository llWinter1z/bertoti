# Engenharia-de-Software-I
Atividades realizadas durante a aula de Engenharia de Software I, no segundo semestre de 2024.



<h2>* Atividade 1: comentário do livro de engenharia de software no google:</h2>

Engenharia de software, diferente da programação, inclui decisões importantes para o desenvolvimento do software a ser produzido, que deve ser entendido e gerenciado ao longo do tempo. Além de possuir os conhecimentos de programação, é necessário que o engenheiro realize escolhas quanto às necessidades de seu programas, abordando decisões mais estratégicas e cuidadosas.

Além disso, a engenharia de software deve empregar uma visão mais ampla quanto à programação, devido a maior escala na qual os sistemas são utilizados.

E por fim, as escolhas tomadas pelos engenheiros de software são de extrema importância, pois são de maior complexidade e impacto, e muitas vezes são estimadas a partir de informações imprecisas, reunidas com o passar do tempo.



<h2>* Atividade 2: Três exemplos de trade-off's citando requisitos não-funcionais:</h2>

<h3>Exemplo 1: C x Python (Desempenho x Produtividade):</h3>

C é mais eficiente e quanto ao desempenho e controle de software, devido a sua baixa ocupação de memória, porém, requer mais tempo e esforço para ser utilizado em desenvolvimento de softwares.

Por outro lado, o Python, apesar de menos eficiente que o C em termos de desempenho, permite um desenvolvimento mais rápido e fácil, devido ao número de bibliotecas e a sintaxe simples.

<h3>Exemplo 2: Rust x JavaScript (Segurança x Flexibilidade):</h3>

A compilação em Rust garante uma maior segurança devido ao seu foco intenso em segurança de memória e concorrência. No entanto, a sua rigidez pode significar mais trabalho aos desenvolvedores, diminuindo a sua flexibilidade com estes.

O JavaScript, por sua vez, tem uma flebilidade maior devido a sua natureza dinâmica e a quantidade vasta de bibliotecas que ela pode oferecer. Contudo, essa mesma natureza pode significar mais vulnerabilidades em sua segurança.

<h3>Exemplo 3: Scala x C++ (Manutenção x Performance):</h3>

A sintaxe limpa, a combinação de programação funcional e orientada a objetos, e as ferramentas de análise de código da Scala, dão a possibilidade de um melhor entendimento e modificação dos códigos produzidos, levando a uma melhor capacidade de manutenção a longo prazo. Apesar disso, em casos onde há um intensivo uso de recursos, a Scala apresenta performance inferior ao C++.

Já o C++, facilita as execuções de códigos devido ao sua alta performance, em detrimento de sua capacidade de ser mantida, em razão de sua complexidade e gerenciamento de memória.



<h2>* Atividade 3: Escolher a arquitetura de uma empresa e comentar seus tradeoffs:</h2>

![Twitter](https://github.com/llWinter1z/Engenharia-de-Software-I/blob/main/Twitter_System_Design.png?raw=true)

<h3>Complexidade de Gerenciamento:</h3>

A arquitetura de microserviços, embora escalável, aumenta a complexidade de gerenciamento. Cada serviço precisa ser monitorado, mantido e atualizado independentemente, o que pode ser desafiador.

<h3>Consistência e Disponibilidade:</h3>

Em sistemas distribuídos, há um trade-off entre consistência e disponibilidade. O Twitter prioriza a disponibilidade para garantir que o serviço esteja sempre acessível, mesmo que isso signifique que algumas atualizações de dados possam não ser imediatamente consistentes.

<h3>Latência:</h3>

O uso de caches e tecnologias de streaming ajuda a reduzir a latência, mas também introduz complexidade adicional na sincronização de dados e no gerenciamento de falhas.

<h3>Escalabilidade Horizontal:</h3>

Embora a escalabilidade horizontal permita que o Twitter lide com picos de tráfego adicionando mais servidores, isso também requer uma infraestrutura robusta de balanceamento de carga e clustering para distribuir eficientemente a carga de trabalho



<h2>* Atividade 4: Fazer classes UML ao lado de código java mostrando a relação entre eles:o</h2>

<pre>
<code>
package atividade4;

import java.util.List;
import java.util.LinkedList;
/**
 *
 * @author fabio
 */
public class ClienteCompra {
    public class Cliente {
        private String nome;
        private int id;
        private List<Items> compras;

        public String getNome() {
        return nome;
        }

        public int getId() {
        return id;
        }

        public List<Items> getCompras() {
        return compras;
        }

        public void setNome(String nome) {
        this.nome = nome;
        }

        public void setId(int id) {
        this.id = id;
        }

        public void setCompras(List<Items> compras) {
        this.compras = compras;
        }
    }
    
    public class Items {
        private int idItem;
        private int nomeItem;
    }
}
</code>
</pre>
