# Make-mobs-fight-each-other-1.18.2

package net.mcreator.testmod.procedures;

import net.minecraftforge.fml.common.Mod;
import net.minecraftforge.eventbus.api.SubscribeEvent;
import net.minecraftforge.eventbus.api.Event;
import net.minecraftforge.event.entity.living.LivingEvent;

import net.minecraft.world.phys.Vec3;
import net.minecraft.world.phys.AABB;
import net.minecraft.world.level.LevelAccessor;
import net.minecraft.world.entity.Mob;
import net.minecraft.world.entity.Entity;
import net.minecraft.world.entity.player.Player;
import net.minecraft.world.entity.LivingEntity;
import net.minecraft.world.level.LevelAccessor;
import net.minecraft.world.level.GameType;
import net.minecraft.server.level.ServerPlayer;
import net.minecraft.client.Minecraft;

import net.mcreator.testmod.init.TestModModGameRules;




import javax.annotation.Nullable;

import java.util.stream.Collectors;
import java.util.List;
import java.util.Comparator;
import java.util.jar.Attributes;

@Mod.EventBusSubscriber
public class ThjProcedure {
	@SubscribeEvent
	public static void onEntityTick(LivingEvent.LivingUpdateEvent event) {
		execute(event, event.getEntityLiving().level, event.getEntityLiving().getX(), event.getEntityLiving().getY(), event.getEntityLiving().getZ(),
				event.getEntityLiving());
	}

	public static void execute(LevelAccessor world, double x, double y, double z, Entity entity) {
		execute(null, world, x, y, z, entity);
	}

	private static void execute(@Nullable Event event, LevelAccessor world, double x, double y, double z, Entity entity) {
	    if(0 == 0){
	    boolean target_once = false;
	    int attack_dist = 0;
	    Entity storedEntity = entity;
		if (entity == null)
		return;
		if (entity instanceof Mob mobB && entity instanceof LivingEntity entityA) {
		if(!(mobB.isAggressive())){
		if(world.getLevelData().getGameRules().getBoolean(TestModModGameRules.MADMOBSMODE)){
		if (entity instanceof Mob) {

		        if(entity instanceof Mob mobA){
				final Vec3 _center = new Vec3(x, y, z);
				List<Entity> _entfound = world.getEntitiesOfClass(Entity.class, new AABB(_center, _center).inflate((Math.random() * 64) / 2d), e -> true)
					.stream().sorted(Comparator.comparingDouble(_entcnd -> _entcnd.distanceToSqr(_center))).collect(Collectors.toList());
				for (Entity entityiterator : _entfound) {
				    if(entity instanceof Mob mob && entityiterator instanceof LivingEntity entity_){
				     if((entity instanceof Mob _mobEnt ? (Entity) _mobEnt.getTarget() : null) == entity_){
					   target_once = true;
					   storedEntity = entityiterator;
					 }
				     if(!(entity == entityiterator)){
				     if(target_once == false || target_once == true && entityiterator == storedEntity){
				     	 if(!(target_once)){
				     	 }
				         target_once = true;
				     if(!(entityiterator instanceof Player)){
					mob.setTarget(entity_);

				     }else{
				     	if (world.getLevelData().getGameRules().getBoolean(TestModModGameRules.MADMOBSMODE)) {
			if (new Object() {
				public boolean checkGamemode(Entity _ent) {
					if (_ent instanceof ServerPlayer _serverPlayer) {
						return _serverPlayer.gameMode.getGameModeForPlayer() == GameType.SURVIVAL;
					} else if (_ent.level.isClientSide() && _ent instanceof Player _player) {
						return Minecraft.getInstance().getConnection().getPlayerInfo(_player.getGameProfile().getId()) != null && Minecraft
								.getInstance().getConnection().getPlayerInfo(_player.getGameProfile().getId()).getGameMode() == GameType.SURVIVAL;
					}
					return false;
				}
			}.checkGamemode(entity_)) {
				if (entity_ instanceof ServerPlayer _player){
					mob.setTarget(_player);
			}
				     }
				     	}
				    }
				}
				}
				     }
		        }
			  } 
		     }
		}
			}
		  }
		}
		}
