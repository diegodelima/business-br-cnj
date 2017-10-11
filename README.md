Module Version: 0.02

NAME ^

Business::BR::CNJ - Harness brazilian CNJ (Conselho Nacional de Justiça) data and functions.

SYNOPSIS ^

use Business::BR::CNJ ( qw/ cnj_check_number / );

cnj_check_number('0058967-77.2016.8.19.0000') || die 'Wrong number!';

# or...

use Business::BR::CNJ;

Business::BR::CNJ::cnj_check_number('0058967-77.2016.8.19.0000') || die 'Wrong number!';
DESCRIPTION ^

This module handles CNJ numbers and data.

METHDOS ^

cnj_check_number

Checks if a process number is numerically valid or not.

References:

http://www.cnj.jus.br/busca-atos-adm?documento=2748

§ 2º O campo (DD), com 2 (dois) dígitos, identifica o dígito verificador, cujo cálculo de verificação deve ser efetuado pela aplicação do algoritmo Módulo 97 Base 10, conforme Norma ISO 7064:2003, nos termos das instruções constantes do Anexo VIII desta Resolução.

Art. 1º Fica instituída a numeração única de processos no âmbito do Poder Judiciário, observada a estrutura NNNNNNN-DD.AAAA.J.TR.OOOO, composta de 6 (seis) campos obrigatórios, nos termos da tabela padronizada constante dos Anexos I a VII desta Resolução.

SEE ALSO ^

Please check CNJ website at http://www.cnj.jus.br/

AUTHOR ^

Diego de Lima, diego_de_lima@hotmail.com

SPECIAL THANKS ^

This module was kindly made available by the https://modeloinicial.com.br/ team.

COPYRIGHT AND LICENSE ^

Copyright (C) 2017 by Diego de Lima

This library is free software; you can redistribute it and/or modify it under the same terms as Perl itself, either Perl version 5.10.1 or, at your option, any later version of Perl 5 you may have available.
