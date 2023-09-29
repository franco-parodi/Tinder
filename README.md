/*@startuml
class mensaje{}

class Perfil{
private nombre:string;
private descripcion: string;
private foto: string;
private dominio: Dominio
private tipoPerfil: TipoPerfil;
private coleccionDeRTA: rta[];

}

class Like{
private likeador: Perfil;
private likeado: Perfil;
private timeStamp: Date;
}

class Match{
private  likes: Like[];
private timeStamp: Date;
}


class Dominio{
private nombre:string;
private tipoVinculacion: TipoVinculaciones;
private cantParticipantes: number;
private tiposPerfiles: TipoPerfil [];
private camposVariables: CampoVariable[];
}

class TipoPerfil{
private nombre: string
}


class CampoVariable{
private nombre: string;
private posiblesValores: PosibleValor[];
private campoObligatorio: boolean
}

class PosibleValor{
private descripcion:string;
}

class rta{
private campoVariable: CampoVariable;
private posibleValor: PosibleValor;
}

enum TipoVinculaciones{
SIMPLE,
MULTIPLE;
}
@enduml*/