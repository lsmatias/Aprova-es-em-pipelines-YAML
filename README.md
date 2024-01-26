# Aprovações em Pipelines-YAML

Uma implantação totalmente autônoma do software em desenvolvimento é desejável, mas às vezes são necessárias aprovações manuais. O Azure DevOps oferece duas maneiras em pipelines YAML para informar os usuários e interromper a execução até que a aprovação seja concedida:

## Aprovações em Ambientes:

Se ambientes já estiverem definidos (ou se devem ser usados), um Approval Check pode ser anexado a um ambiente. Antes da implantação em um ambiente, verifica-se se todos os checks foram concluídos. Caso contrário, a execução é interrompida até que a aprovação seja concedida.

## Tarefa de Validação Manual (Manual Validation) diretamente em um Pipeline YAML:

Também é possível usar a tarefa "Manual validation" diretamente em um pipeline YAML. Essa tarefa interrompe a execução do pipeline na etapa ou trabalho atual até que uma aprovação seja concedida. É possível continuar o pipeline mesmo se a aprovação não for concedida. Observação: A tarefa "Manual validation" (waitForValidation@0) ainda está em Preview.

![ManualValidation@0 – Manual validation v0 task](https://learn.microsoft.com/en-us/azure/devops/pipelines/tasks/reference/manual-validation-v0?view=azure-pipelines)


![Define approvals and checks](https://learn.microsoft.com/en-us/azure/devops/pipelines/process/approvals?view=azure-devops&tabs=check-pass#approvals)


<img width="495" alt="image" src="https://github.com/lsmatias/Aprova-es-em-pipelines-YAML/assets/28391885/8d78c702-5cda-482d-b6ef-01b325661a17">


<img width="489" alt="image" src="https://github.com/lsmatias/Aprova-es-em-pipelines-YAML/assets/28391885/b5a98d16-abc7-4bf7-8c66-b325eab48e05">


<img width="490" alt="image" src="https://github.com/lsmatias/Aprova-es-em-pipelines-YAML/assets/28391885/bc688cbc-248f-454b-8dcc-0c6a80d3f3f6">


<img width="868" alt="image" src="https://github.com/lsmatias/Aprova-es-em-pipelines-YAML/assets/28391885/7c10e653-2800-40ce-b567-5c3c333514f9">




