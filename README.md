# Kyverno Policies

Este repositório contém políticas (policies) para o Kyverno, uma ferramenta de política nativa do Kubernetes. O Kyverno permite definir políticas declarativas para a validação e mutação de recursos Kubernetes. As políticas aqui fornecidas visam ajudar na aplicação consistente de práticas de segurança, conformidade e melhores práticas em clusters Kubernetes.

Kyverno é uma ferramenta de gerenciamento de políticas para Kubernetes, focada na automação de várias tarefas relacionadas à segurança e configuração dos clusters de Kubernetes. Ele permite que você defina, gerencie e aplique políticas de forma declarativa para garantir que os clusters e suas cargas de trabalho estejam em conformidade com as regras e normas definidas.

**Principais Funções do Kyverno:**

Validação de Recursos: Verifica se os recursos do Kubernetes estão em conformidade com as políticas definidas. Por exemplo, pode garantir que todos os Pods tenham limites de CPU e memória definidos.

Mutação de Recursos: Modifica automaticamente os recursos do Kubernetes para atender às políticas definidas. Por exemplo, pode adicionar automaticamente labels específicos a todos os novos Pods.

Geração de Recursos: Cria recursos adicionais do Kubernetes com base nas políticas definidas. Por exemplo, pode gerar NetworkPolicies para cada novo Namespace criado.




## Estrutura do Repositório 
- **/policies** : Este diretório contém as políticas Kyverno no formato YAML. Cada política é projetada para endereçar uma preocupação específica, como controle de acesso, segurança de imagem, entre outros.
- **/docs** :Este diretório contém a documentação relacionada ao uso e contribuição para as políticas Kyverno.
- 
## Como Usar
1. Clone este repositório para o seu ambiente local ou diretamente em seu cluster Kubernetes.

```bash
git clone https://github.com/Tech-Preta/kyverno-policies.git
cd kyverno-policies
```

 
1. Aplique as políticas desejadas ao seu cluster usando o comando `kubectl apply`:

```bash
kubectl apply -f policies/minha-politica.yaml
```


1. Verifique se as políticas foram aplicadas corretamente:

```bash
kubectl get policies
```


## Contribuindo

Se você quiser contribuir com novas políticas, correções ou melhorias, sinta-se à vontade para criar um fork deste repositório e enviar um pull request.

Certifique-se de seguir as diretrizes de contribuição do projeto e testar suas alterações localmente antes de enviar uma solicitação de mesclagem.



